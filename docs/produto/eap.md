# Estrutura Analítica do Projeto (EAP)

## 1. Introdução

De acordo com o PMBOK, a Estrutura Analítica do Projeto (EAP), também conhecida como Work Breakdown Structure (WBS), é a decomposição hierárquica do escopo total do trabalho a ser executado pela equipe do projeto para atingir os objetivos e gerar as entregas requeridas. A EAP organiza e define o escopo total do projeto, sendo um artefato central para o planejamento, execução e controle.

No contexto do MeasureSoftGram 2026.1, a EAP foi elaborada no formato de MVP Canvas, organizando as entregas em **ondas** — conjuntos de funcionalidades agrupadas por tema e priorizadas sequencialmente, baseadas nos resultados da Lean Inception da equipe.

## 2. EAP do Projeto

<iframe
  src="../../assets/eap-viewer.html"
  width="100%"
  height="520px"
  style="border: 1px solid #e0e0e0; border-radius: 8px;">
</iframe>

## 3. Descrição das Ondas e Sub-níveis

### Onda 1 — OnBoarding
**Período:** 13/04/2026 a 27/04/2026

A primeira onda concentra as atividades de nivelamento da equipe, planejamento inicial do projeto e configuração da infraestrutura base. O objetivo é garantir que todos os membros estejam alinhados com a visão do produto e que o ambiente de desenvolvimento esteja pronto para as entregas subsequentes.

| Entrega | Descrição |
|---------|-----------|
| **DOCS: Atualizar docs separado por repositório** | Atualização e organização da documentação técnica de cada repositório do MeasureSoftGram de forma independente, garantindo rastreabilidade e onboarding facilitado. |
| **PRODUTO: Definição da Visão do Produto** | Definição clara da visão, propósito e proposta de valor do produto MeasureSoftGram para o semestre 2026.1, alinhando todos os stakeholders. |
| **PRODUTO: Personas e Jornadas de Usuário** | Identificação e mapeamento das personas e suas jornadas de uso do produto, embasando decisões de desenvolvimento centradas no usuário. |
| **PRODUTO: Brainstorming e Revisão Técnica, de Negócio e UX** | Sessão de brainstorming de funcionalidades seguida de revisão técnica, de negócio e de experiência do usuário para validar viabilidade e valor. |
| **PRODUTO: Sequenciador, MVP e Priorização Inicial** | Uso do sequenciador da Lean Inception para priorizar funcionalidades e definir o escopo mínimo viável (MVP) para o semestre. |
| **GESTÃO: Planejamento e Governança do Projeto** | Planejamento geral do projeto com definição de papéis, cerimônias ágeis, ferramentas e práticas de governança da equipe. |
| **GESTÃO: Comunicação e Acompanhamento de Sprints** | Estabelecimento de canais de comunicação e rotinas de acompanhamento de progresso das sprints ao longo do semestre. |
| **US01: Configurar Dockerhub** | Configuração do repositório de imagens Docker no DockerHub para facilitar o deploy e a distribuição dos componentes do MeasureSoftGram. |
| **US02/03: Action Local e Docker** | Configuração do ambiente local para execução da GitHub Action do MeasureSoftGram, incluindo suporte a Docker para execução isolada e reprodutível. |

---

### Onda 2 — Integração e IA
**Período:** 27/04/2026 a 11/05/2026

A segunda onda foca na evolução das integrações existentes e na introdução das primeiras capacidades de Inteligência Artificial ao produto. São entregues melhorias de segurança, usabilidade e a base da integração com o Claude AI via protocolo MCP.

| Entrega | Descrição |
|---------|-----------|
| **US04: Atualizar Marketplace** | Atualização da publicação da GitHub Action no marketplace oficial do GitHub, incluindo metadados, descrição e documentação de uso atualizados. |
| **US05: Criptografar Senhas** | Implementação de criptografia robusta para armazenamento e transmissão de senhas dos usuários, aumentando a segurança do sistema. |
| **US06: Gerenciar Timeout** | Implementação de mecanismo de gerenciamento de timeout para sessões de usuário, melhorando segurança e experiência de uso da plataforma. |
| **US07: Notificar Expiração** | Desenvolvimento de sistema de notificação para alertar usuários sobre a expiração iminente de sessões ou tokens de acesso. |
| **US08: Melhorar CLI** | Aprimoramento da interface de linha de comando (CLI) com novos recursos, mensagens de ajuda aprimoradas e melhor usabilidade geral. |
| **US09: Listar Repositórios** | Implementação de funcionalidade para listar repositórios disponíveis integrados ao MeasureSoftGram, permitindo navegação e seleção facilitada. |
| **US10: Autenticar com GitHub** | Integração de autenticação OAuth com o GitHub para permitir que usuários acessem o sistema usando suas credenciais da plataforma. |
| **US11: Selecionar Repos** | Implementação de interface para seleção de repositórios do GitHub a serem monitorados e analisados pelo MeasureSoftGram. |
| **US12: Integrar MCP Claude** | Integração do protocolo MCP (Model Context Protocol) com o Claude AI para possibilitar análise inteligente de qualidade de software. |

---

### Onda 3 — Expansão e Visualização
**Período:** 11/05/2026 a 25/05/2026

A terceira onda expande as capacidades de análise com IA e introduz novas formas de visualização de dados. O foco está em tornar os insights gerados pela plataforma mais acessíveis e acionáveis para os usuários.

| Entrega | Descrição |
|---------|-----------|
| **US13: Enviar Contexto** | Desenvolvimento de mecanismo para envio de contexto do repositório e suas métricas ao modelo Claude AI para análise aprofundada. |
| **US14: Exibir Respostas** | Implementação de interface para exibição das respostas geradas pela IA a partir do contexto do repositório analisado. |
| **US15: Inserção Atômica** | Implementação de mecanismo de inserção atômica de dados para garantir consistência e integridade nas operações de banco de dados. |
| **US16: Gerar Badge Status** | Desenvolvimento de funcionalidade para geração de badges dinâmicos de status de qualidade para exibição em repositórios GitHub. |
| **US17: Expor API Token** | Implementação de endpoint para geração e gestão de tokens de API, permitindo integrações externas autenticadas com o MeasureSoftGram. |
| **US18: Métricas Kibana** | Integração com o Kibana para visualização e análise de métricas coletadas pelo MeasureSoftGram em dashboards interativos. |
| **US19: Agente Interativo** | Desenvolvimento de agente de IA interativo para responder perguntas e fornecer análises sobre a qualidade do software em tempo real. |
| **US20: Relatórios Analíticos** | Criação de relatórios analíticos detalhados sobre qualidade do software, tendências e comparações entre releases. |
| **US21: Resumo Executivo** | Geração automática de resumos executivos sobre o estado da qualidade do software para apresentação a gestores e stakeholders. |

---

### Onda 4 — Extensões e Qualidade
**Período:** 25/05/2026 a 08/06/2026

A quarta onda entrega extensões avançadas do produto e aprimora as métricas de qualidade disponíveis. Novas formas de visualização e integração com ferramentas externas ampliam o alcance da plataforma.

| Entrega | Descrição |
|---------|-----------|
| **US22: Gráfico Semáforo** | Implementação de visualização em formato de semáforo para indicar o status de qualidade de forma intuitiva e de fácil interpretação por qualquer perfil de usuário. |
| **US23: Modelo AHP** | Integração do método AHP (Analytic Hierarchy Process) para ponderação e priorização de características de qualidade do software de forma estruturada. |
| **US24: Plugin VSCode IA** | Desenvolvimento de plugin para o Visual Studio Code que integra as funcionalidades de IA do MeasureSoftGram diretamente no ambiente de desenvolvimento. |
| **US25: Visualizar Grafana** | Integração com o Grafana para visualização avançada de métricas e dashboards de qualidade de software em tempo real. |
| **US26: Calcular Qualidade Uso** | Implementação de algoritmo para calcular métricas de qualidade de uso baseadas em dados reais de utilização do sistema pelos usuários. |
| **US27: Exibir Características** | Desenvolvimento de interface detalhada para exibição das características de qualidade do software analisadas pelo MeasureSoftGram. |
| **US28: Loading Detalhado** | Implementação de indicadores de progresso detalhados durante operações demoradas para melhorar a experiência e transparência ao usuário. |
| **US29: Gráficos CLI** | Adição de suporte à visualização de gráficos e métricas diretamente na interface de linha de comando, sem necessidade de interface gráfica. |

---

### Onda 5 — MVP Consolidado
**Período:** 08/06/2026 a 22/06/2026

A quinta onda consolida o MVP com as funcionalidades de presets e integração de IA no pipeline, tornando o produto completo para uso em contextos reais de engenharia de software.

| Entrega | Descrição |
|---------|-----------|
| **US30: Configurar Presets** | Implementação de sistema de presets configuráveis para padronizar análises de qualidade conforme diferentes contextos, projetos e organizações. |
| **US31: Presets na Release** | Integração dos presets de configuração no fluxo de release, permitindo análises automáticas parametrizadas em cada entrega do produto. |
| **US32: IA no Pipeline** | Integração de análises de IA diretamente no pipeline de CI/CD para fornecer feedback automático sobre qualidade durante o desenvolvimento. |
| **US33: Novos Modelos Base** | Adição de novos modelos de referência para avaliação de qualidade de software, expandindo as opções de análise disponíveis para diferentes domínios. |
| **US34: Refatorar Equalizador** | Refatoração do componente equalizador de métricas para melhorar performance, manutenibilidade e extensibilidade do módulo. |

---

### Onda 6 — Ajustes e Docs
**Período:** 22/06/2026 a 06/07/2026

A sexta e última onda é dedicada à consolidação da documentação técnica e dos prompts de IA, garantindo que o produto seja sustentável, documentado e mantível pelas próximas equipes.

| Entrega | Descrição |
|---------|-----------|
| **US35: Docs de Arquitetura** | Criação e atualização de documentação técnica de arquitetura para todos os repositórios do MeasureSoftGram, facilitando onboarding futuro. |
| **US36: Docs e Prompts IA** | Documentação completa dos prompts e fluxos de IA utilizados no MeasureSoftGram, facilitando manutenção e evolução das integrações. |

---

## 4. Resumo das Ondas

| Onda | Tema | Período | Entregas |
|------|------|---------|----------|
| Onda 1 | OnBoarding | 13/04 – 27/04 | Docs, Produto, Gestão, US01, US02/03 |
| Onda 2 | Integração e IA | 27/04 – 11/05 | US04 a US12 |
| Onda 3 | Expansão e Visualização | 11/05 – 25/05 | US13 a US21 |
| Onda 4 | Extensões e Qualidade | 25/05 – 08/06 | US22 a US29 |
| Onda 5 | MVP Consolidado | 08/06 – 22/06 | US30 a US34 |
| Onda 6 | Ajustes e Docs | 22/06 – 06/07 | US35 e US36 |

## 5. Versionamento do Documento

| Data | Versão | Descrição | Autor |
|------|--------|-----------|-------|
| 25/04/2026 | 1.0 | Criação do documento de EAP 2026.1 | [DeM4rcio](https://github.com/DeM4rcio) |
