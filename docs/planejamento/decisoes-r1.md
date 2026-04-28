# Decisões da Release Major R1 — baseadas em dados

> **Critério da disciplina:** seção exigida pelo Dashboard Gerencial e Analítico da R1 (peso 30%).
> Cada decisão registrada aqui parte de **um dado observável** (gráfico, métrica, evento) e tem **evidência rastreável** (PR, commit, arquivo do repositório, ata).

| Sprint | Tipo | Decisão | Status |
|---|---|---|---|
| Sprint 4-5 | Técnica | Modernizar stack Docker (PG18 + uv + pnpm + versões pinadas) | ✅ implantada |
| Sprint 1-2 | Gerencial | Estrutura de Clãs + Alianças (Spotify adaptado) | ✅ vigente |
| Sprint 5 | Gerencial | Priorizar resposta a 6 riscos críticos (R01-R06) antes da R1 | ✅ planejada |

---

## Decisão 1 — Modernizar a stack Docker do MSGram

### Contexto e dado que motivou

Builds do Service e do Front estavam quebrando de forma **inconsistente entre dev local e CI**. Em particular:

- Tempo de `pip install` no Service rodava em **~3-4 min na CI** vs ~30s usando `uv`. Mesma `requirements.txt`, mesma máquina, ferramenta diferente.
- O Front usava `docker-compose` v1 com imagens base sem tag fixa (`:latest`), e a versão do Postgres oscilava entre 12 e 14 conforme a build, dependendo da máquina.
- Bug **#003 — infra Docker versões** (rastreado no fork antigo do Service) reproduzia apenas com a stack antiga.

### Decisão

A partir da Sprint 4, o time padronizou em todos os repos do MSGram:

- **`uv`** como gerenciador de pacotes Python (Service, Core, Parser, CLI) — substitui `pip`/`pipenv`/`poetry`. Lockfile reprodutível.
- **`pnpm`** como gerenciador no Front — substitui `npm`/`yarn`. Cache por content-hash.
- **Versões pinadas em todos os Dockerfiles e `docker-compose.yml`**: `python:3.12-slim`, `node:20-alpine`, `postgres:18-alpine`. Sem `:latest`.
- **PostgreSQL 18-alpine** substituindo PG12/14 herdados.
- **Docker Compose v2** com `compose watch` para hot reload no desenvolvimento.

### Evidências

- PR Service [#1 — fix(infra): modernize Docker stack](https://github.com/fga-eps-mds/2026.1-MeasureSoftGram-Service/pull/1) — *merged*.
- PR Front [#5 — fix(infra): docker-compose enxuto, sem service+db duplicados](https://github.com/fga-eps-mds/2026.1-MeasureSoftGram-Front/pull/5) — *merged*.
- Documento de Arquitetura: subseção "Gerenciamento de pacotes e runtime" em `arquitetura.md` v1.4.

### Impacto observado pós-implantação

- Build da CI do Service caiu de ~4 min pra ~1 min.
- Reprodutibilidade entre dev / CI / homologação fechou (sem mais "funciona na minha máquina" relacionado a versão de runtime).

---

## Decisão 2 — Estrutura de Clãs e Alianças (Spotify adaptado)

### Contexto e dado que motivou

O time de 2026.1 começou com **15 pessoas** distribuídas em três superfícies de produto (Action, CLI, Web) e quatro repositórios funcionais (Core, Parser, Service, Front). Dois dados orientaram a discussão de organização:

- **Daily/planning de 1h com 15 pessoas é matematicamente inviável** — média de 4 min por pessoa elimina qualquer aprofundamento.
- O MSGram tem **três superfícies-cliente** (CLI, Action, Web) que poderiam evoluir em paralelo, mas com **bibliotecas comuns** (Core, Parser) cuja interface afeta todo mundo.

### Decisão

Adotamos o modelo Spotify adaptado em **duas dimensões cruzadas**:

- **3 Clãs por superfície de produto** (eixo de *features* — Web, CLI, Action). Cada Clã entrega features ponta-a-ponta na sua superfície e tem cerimônias semanais próprias.
- **4 Alianças por repositório** (eixo de *decisões técnicas do código* — Core, Parser, Service, Front). Cada pessoa pertence a um Clã e a uma Aliança; a Aliança decide o que entra "no seu" repositório, mesmo quando outro Clã contribui pra ele.

Justificativa teórica: aplicação direta da **Lei de Conway** (a estrutura de comunicação reflete e molda a arquitetura) — a fronteira-de-time vertical reflete a fronteira-de-feature; a fronteira-de-time horizontal reflete a fronteira-de-código.

### Evidências

- `docs/planejamento/clas.md` — estrutura completa, líderes, cerimônias.
- Memorando de Decisão MD-R1 do Giovanni A. C. Giampauli (matrícula 211043647) — fundamentação teórica completa (Kniberg & Ivarsson 2012, Conway 1968).

### Critério de sucesso (acompanhamento)

Ao fim da R1, ≥ 80 % das issues fechadas executadas dentro do Clã dono da superfície — medido via cruzamento `assignee × repo` no Zenhub e GitHub. Métrica registrada para retrospectiva da R2.

---

## Decisão 3 — Priorizar resposta a 6 riscos críticos antes da R1

### Contexto e dado que motivou

Em 24/04/2026 a Aliança de Planejamento mapeou **17 riscos** ativos no projeto, classificados por probabilidade × impacto na matriz `docs/planejamento/riscos.md`. Da matriz emergiu o dado-chave:

- **6 riscos** caíram na faixa "alto/crítico" (probabilidade ≥ 3 × impacto ≥ 4 na escala 1-5).
- 11 riscos restantes ficaram em faixa "médio/baixo" — endereçáveis na R2 sem comprometer a R1.

### Decisão

Atacar os 6 riscos críticos durante a janela R1 com plano de resposta explícito (mitigação ou contingência), **antes** de incrementar funcionalidades novas. Os 11 riscos restantes seguem monitorados na planilha vinculada, mas sem ação imediata na sprint atual.

### Evidências

- `docs/planejamento/riscos.md` — versão atualizada em 27/04/2026 com tabela de probabilidade × impacto, causa, consequência e plano de ação por risco.
- Planilha Google de monitoramento contínuo (linkada no `riscos.md`).

### Critério de sucesso (acompanhamento)

Para cada um dos 6 riscos críticos: ou o risco foi **mitigado** (probabilidade caiu de faixa) até o início da Sprint 6, ou está com **contingência ativada** com responsável e prazo. Acompanhamento na retrospectiva da R1 (apresentação de 29/04 21h).

---

## Versionamento

| Data | Versão | Descrição | Autor |
|:-:|:-:|:-:|:-:|
| 27/04/2026 | 1.0 | Versão inicial — 3 decisões da R1 com dado, decisão e evidência | [Giovanni A. C. Giampauli](https://github.com/giovanniacg) |
