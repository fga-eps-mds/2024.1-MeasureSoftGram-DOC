# Plano de Custos

## Introdução

É fundamental para um projeto ter um plano de custos bem definido. Um plano de custos claro e eficiente permite representar os gastos previstos do projeto, possibilitando que o cliente avalie se o projeto cabe em seu orçamento. Além disso, tal plano detalha onde cada quantia será investida e em qual momento ocorrerão as demandas orçamentárias, facilitando a gestão financeira e a tomada de decisões. [<a href=./#referencias-bibliograficas>1</a>]

## Estimativa de custos


### Infraestrutura

Para estimar os custos referentes a infraestrutura, dois elementos forma levados em consideração: fornecimento de energia elétrica e internet.

#### Energia Elétrica

De acordo com a Neoenergia, fornecedora de energia elétrica do Distrito Federal, a tarifa residencial para um quilowatt-hora (kWh) é de aproximadamente R$ 0,77. [<a href=./#referencias-bibliograficas>2</a>]

Assumindo que um computador ligado por uma hora, todos os dias, consome 5 kWh por mês [<a href=./#referencias-bibliograficas>3</a>]. Para este projeto, em que cada membro irá trabalhar em média duas horas por dia, o custo com energia elétrica ficará em torno de R$ 1,79 por semana, para cada membro da equipe.

- Consumo médio de um computador por hora: 5 kWh ÷ 30 dias = 0,167
- Consumo de um computador neste projeto por uma semana: 7 dias x 2 horas x 0,167 = 2,33 kWh
- Valor do consumo semanal de energia elétrica: 2,33 kWh x R$ 0,77 = **R$ 1,79**

#### Internet

Assumindo um valor médio de R$ 100,00 para um plano de internet banda larga mensal e 14 horas trabalhadas por pessoa no projeto semanalmente, podemos realizar os seguintes cálculos:

- Quantidade de horas no mês: 30 dias x 24 horas = 720 horas
- Valor do plano de internet por hora: R$ 100,00 ÷ 720 horas = R$ 0,14
- Valor gasto com internet por pessoal semanalmente: **R$ 1,94**

### Equipamentos

Foi considerado como mínimo para desenvolvimento deste projeto, um computador com ao menos 8GB de memória RAM e processador Intel Core i5 ou AMD Ryzen 5. Com essas especificações, foi encontrado na loja "KaBum!" um [notebook](https://www.kabum.com.br/produto/510065/notebook-asus-vivobook-x1502za-ej1761-intel-core-i5-12450h-2ghz-8gb-ram-placa-intel-uhd-graphics-ssd-256gb-tela-15-6-led-full-hd-linux-keepos-prata) com o valor de **R$ 2.518,39** no dia da consulta.

Tendo em mente que os gastos com equipamentos só serão realizados uma vez, para cada membro, durante todo o projeto. Temos o gasto fixo estimado de:

- R$ 2.518,39 x 10 membros = **25.183,90**

### Pessoa

Para estimar o gasto com pessoas, foi considerado o valor anual médio de R$ 19.766,00 para um estudante de universidade federal, esse valor foi encontrado a partir de um estudo feito em 2022 analisando dados do ano de 2019 [<a href=./#referencias-bibliograficas>4</a>]. Levando em consideração a inflação do ano de 2024, este valor seria equivalente hoje a R$ 31.944,32. Assumindo que um estudante universitário cursa em média 40 créditos ao ano, temos:

- Custo por crédito: R$ 31.944,32 / 40 = R$ 798,61
- Quantidade de créditos de EPS: 4
- Custo de um aluno da disciplina de EPS: R$ 798,61 x 4 = R$ 3.194,43
- Quantidade de Semanas no Projeto: 17
- Custo por semana: R$ 3.194,43 / 17 semanas = **R$ 187,91**

## Planilha de custos

Todos os cálculos realizados foram documentados na seguinte planilha:

<iframe width="1200" height="600" style="-webkit-transform:scale(0.8);-moz-transform-scale(0.8);" frameborder="0" scrolling="yes" src="https://docs.google.com/spreadsheets/d/1F-C_GpFWzMUNv7hoE89GK0adVZlp3T7t5v96rYjhEpw/edit?gid=0#gid=0"></iframe>

Com isso, obtemos um custo total de **R$ 61.430,93** para o projeto.

## Agile Earned Value Management (AgileEVM)

A técnica de Earned Value Management (EVM) é um método para integrar escopo, custo e tempo [<a href=./#referencias-bibliograficas>5</a>]. O EVM assume um determinado escopo, para a partir dele definir o custo e tempo, portanto uma abordagem que atende melhor o contexto de projetos ágeis é o Agile Earned Value Management (AgileEVM), uma versão adaptada do EVM tradicional, porém utilizando métricas do Scrum [<a href=./#referencias-bibliograficas>6</a>].

As tabelas do contendo todos os cálculos e valores utilizados para gerar o AgileEVM está disponível abaixo.

<iframe width="1200" height="600" style="-webkit-transform:scale(0.8);-moz-transform-scale(0.8);" frameborder="0" scrolling="yes" src="https://docs.google.com/spreadsheets/d/1tcyKBuUES50fDaddEJEe1krEmYhTU_qx_1XLjk22ZBQ/edit?gid=518402925#gid=518402925"></iframe>

## Referências Bibliográficas
> [1] Plano de gerenciamento de custos: como os CFOs devem atuar?. Disponível em: https://www.concur.com.br/blog/article/plano-de-gerenciamento-de-custos. Acesso em: 01 de agosto de 2024

> [2] Composição Tarifária. Disponível em: https://www.neoenergia.com/web/brasilia/sua-casa/composicao-tarifarias. Acesso em: 01 de agosto de 2024

> [3] Dicas para Economizar Energia ao Usar o Computador. Disponível em: https://www.mpgo.mp.br/portal/conteudo/dicas-para-economia-de-energia-ao-usar-o-computador. Acesso em: 01 de agosto de 2024

> [4] Bielschowsky, Carlos Eduardo, e Nelson Cardoso Amaral. “O CUSTO DO ALUNO DAS 2.537 INSTITUIÇÕES DE EDUCAÇÃO SUPERIOR BRASILEIRAS: CAI UM MITO?” Educação & Sociedade, vol. 43, 2022, p. e243866. DOI.org (Crossref), https://doi.org/10.1590/es.243866.

> [5] “Guide to the Project Management Body of Knowledge - PMBOK® Guide 2003 Edition”, Project Management Institute, Pennsylvania, 2003.

> [6] T. Sulaiman, B. Barton, e T. Blackburn, “AgileEVM - Earned Value Management in Scrum Projects”, AGILE 2006 (AGILE’06).
