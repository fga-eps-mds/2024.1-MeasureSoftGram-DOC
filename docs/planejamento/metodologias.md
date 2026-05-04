# Metodologia

## Introdução

<div align="justify">&emsp;&emsp;
A metodologia deste projeto caracteriza-se por uma abordagem híbrida, utilizando o PMBOK como referencial de gestão e governança, enquanto a execução técnica fundamenta-se nos métodos ágeis Scrum e XP e na filosofia Lean para otimização do fluxo de trabalho. Esta seção explica como esses elementos são articulados entre si, não apenas os descrevendo isoladamente, mas evidenciando a lógica de integração que orienta o desenvolvimento do projeto.
</div>

## Referencial de Gestão

### PMBOK

<div align="justify">&emsp;&emsp;
O PMBOK (Project Management Body of Knowledge) é um guia de boas práticas de gerenciamento de projetos publicado pelo Project Management Institute (PMI). Embora seja associado a uma visão tradicional e positivista de gestão, elementos do PMBOK são utilizados neste projeto para estruturar a governança, o planejamento de custos, o gerenciamento de riscos e a organização das entregas. Assim, o PMBOK não é adotado integralmente, mas serve como referencial complementar que confere disciplina e rastreabilidade aos processos de gestão, integrando-se à execução ágil conduzida pelos demais métodos.
</div>

- Gestão de Riscos: Identificação, análise e planejamento de respostas a riscos ao longo do projeto.
- Gestão de Custos: Estimativa e controle dos custos associados ao desenvolvimento.
- Estrutura Analítica do Projeto (EAP): Decomposição hierárquica do escopo do projeto em entregas menores e gerenciáveis.
- Plano de Comunicação: Definição dos canais, frequências e responsáveis pela comunicação entre as partes interessadas.

## Métodos de Desenvolvimento

### Scrum

<div align="justify">&emsp;&emsp;
O Scrum é um framework de gerência de equipes, em que os integrantes do desenvolvimento assumem uma abordagem proativa diante da complexidade e da incerteza que são inerentes aos projetos.
</div>

- Sprints: Prazo de trabalho fixo, em nosso projeto de uma semana, em que são desenvolvidos os incrementos do projeto.
- Planning: As reuniões de planning servem para a definição das metas da sprint.
- Revisão e Retrospectiva: Ao final da sprint são realizadas as cerimônias de revisão e retrospectiva, onde é feita uma análise e documentação do que foi realizado além da sugestão de ideias de melhorias.
- Product Backlog: O backlog de um produto consiste na lista de itens planejados e desenvolvidos pela equipe.

### XP (Extreme Programming)

<div align="justify">&emsp;&emsp;
O Extreme Programming (XP) é um método de desenvolvimento de software que promove a colaboração, a comunicação e a adaptabilidade por meio de um conjunto de práticas de engenharia bem definidas. No projeto, o XP é aplicado de forma ampla, indo além das práticas mais visíveis, e muitas de suas técnicas já se tornaram tão naturais na rotina da equipe que nem sempre são percebidas como pertencentes ao método.
</div>

- Histórias de Usuário (User Stories): Descrições curtas de funcionalidades do ponto de vista do usuário final, utilizadas para compor e priorizar o backlog do produto.
- Planejamento de Entregas (Release Planning): Planejamento de quais histórias serão entregues em cada release, equilibrando valor para o cliente e capacidade da equipe.
- Releases Pequenas (Small Releases): Entregas frequentes e incrementais que permitem a validação contínua do produto pelo cliente sem depender de grandes ciclos de desenvolvimento.
- Integração Contínua (Continuous Integration): Integração frequente do código desenvolvido ao repositório principal, acompanhada de execução automatizada de testes para detectar problemas precocemente.
- Propriedade Coletiva do Código (Collective Ownership): Qualquer membro da equipe pode modificar qualquer parte do código, promovendo responsabilidade compartilhada e reduzindo gargalos.
- Padrões de Codificação (Coding Standards): Adoção de convenções e diretrizes comuns de escrita de código para garantir consistência e legibilidade ao longo do projeto.
- Testes Automatizados (Automated Testing): Escrita de testes automatizados que acompanham o desenvolvimento das funcionalidades, garantindo a qualidade e permitindo refatorações seguras.
- Refatoração (Refactoring): Melhoria contínua da estrutura interna do código sem alterar seu comportamento externo, mantendo a base de código saudável ao longo do tempo.
- Planning Poker: Técnica utilizada para a mensuração do esforço esperado para determinado item a ser trabalhado.

## Filosofia de Fluxo

### Lean e Kanban

<div align="justify">&emsp;&emsp;
O Lean é uma filosofia de gestão e organização de fluxo de trabalho originada na manufatura, cujo princípio central é a eliminação de desperdícios e a maximização de valor entregue. Na área de desenvolvimento de software, o Lean fornece a base conceitual para a gestão visual do trabalho e para a otimização do fluxo de desenvolvimento.
</div>

<div align="justify">&emsp;&emsp;
O que popularmente chamamos de Kanban no desenvolvimento de software é uma adaptação do sistema visual de controle de produção criado pela Toyota dentro do contexto Lean. Em nosso projeto, utilizamos um quadro Kanban — gerenciado pela ferramenta ZenHub — como mecanismo de visualização e controle do fluxo de trabalho, permitindo identificar gargalos, limitar o trabalho em progresso e manter a transparência sobre o andamento das tarefas.
</div>

### Lean Inception

<div align="justify">&emsp;&emsp;
A Lean Inception é um workshop colaborativo, fundamentado nos princípios da filosofia Lean, cujo objetivo é o alinhamento entre as partes interessadas sobre o Produto Mínimo Viável (MVP) a ser desenvolvido. As seguintes atividades compõem o método:
</div>

- Visão do produto: Define uma visão clara e compartilhada do produto.
- É – Não é – Faz – Não faz: Esclarece as características do produto, identificando o que o produto é, o que não é, o que faz e o que não faz.
- Personas: Desenvolve personas representando diferentes perfis de usuários, compreendendo suas necessidades e características.
- Jornada de usuários: Mapeia a jornada dos usuários ao interagir com o produto.
- Brainstorming: Realização de sessões criativas para gerar ideias de funcionalidades e recursos que agreguem valor ao produto.
- Revisão Técnica, de UX e de Negócio: Analisa as ideias geradas e avalia sua viabilidade técnica.
- Sequenciador: Prioriza funcionalidades considerando importância, valor para usuários e viabilidade técnica, criando uma sequência para o desenvolvimento.
- Canvas MVP: Define os elementos essenciais do produto inicial, focando no mínimo necessário para validar o direcionamento do negócio.

## Referências

> PROJECT Management Institute. **A Guide to the Project Management Body of Knowledge (PMBOK® Guide)**. 7. ed. Newtown Square: PMI, 2021.

> O QUE é o Scrum?. [S. l.]. Disponível em: https://aws.amazon.com/pt/what-is/scrum/. Acesso em: 1 ago. 2024.

> O QUE é XP - Extreme Programming?. [S. l.]. Disponível em: Marylene Guedes. Acesso em: 1 ago. 2024.

> EXTREME Programming. [S. l.]. Disponível em: https://www.agilealliance.org/glossary/xp/#:~:text=Extreme%20Programming%20(XP)%20is%20an,engineering%20practices%20for%20software%20development. Acesso em: 1 ago. 2024.

> KANBAN: conceito, como funciona, vantagens e implementação. [S. l.], 3 nov. 2023. Disponível em: https://www.totvs.com/blog/negocios/kanban/. Acesso em: 1 ago. 2024.

> LEAN Inception: Saiba como alinhar pessoas e construir o produto certo. [S. l.], 31 jan. 2022. Disponível em: https://caroli.org/lean-inception-3/. Acesso em: 1 ago. 2024.

## Histórico de Versão

| Versao | Data       | Descricao                                          | Autor           | Revisor                                  |
|--------|------------|----------------------------------------------------|-----------------|------------------------------------------|
| 1.0    | 01/08/2024 | Adição do documento                                | Brenno Oliveira | [João Antonio](https://github.com/i-JSS) |
| 2.0    | 04/05/2026 | Revisão: distinção metodologia/método, PMBOK, XP completo e Lean | Nicollas | — |
