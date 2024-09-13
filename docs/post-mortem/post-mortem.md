# Introdução

O _post mortem_ é uma análise final de um projeto após sua conclusão. O objetivo é revisar os sucessos, desafios, lições aprendidas e identificar pontos pendentes que podem ser desenvolvidos em iterações futuras. No contexto acadêmico, ele também serve para fornecer uma base sólida para que futuros estudantes ou equipes possam continuar o trabalho, evitando a repetição de erros e aprimorando o desenvolvimento.

# Análise da equipe

A equipe, no geral, se sentiu bastante desafiada com a proposta diferente do projeto. A maioria estava acostumada a trabalhar em projetos mais tradicionais, como sistemas de CRUD, onde as operações são claras e diretas. No entanto, com o MeasureSoftwareGram, a ideia de coletar medidas de repositórios e dados específicos, e não apenas gerenciar registros, trouxe uma nova dinâmica para o desenvolvimento.

# Pontos Pendentes

Para construir uma base inicial para os colegas do próximo semestre, a equipe reuniu uma série de pontos pendentes nos repositórios do projeto.

## Característica de Eficiência de Desempenho:

- Criar parser para gerar input a partir dos CSV dos testes de carga
- Preparar banco de dados para salvar dados de testes de carga
- Plugar WEB no CORE para calcular característica
- Definir como serão apresentados os dados na WEB
- Definir como serão inseridos os dados de teste de carga

## Front:

- Remover/alterar componente de carregamento
- Timeout de login para evitar sessão com tempo máximo indefinido
- Passar Hash na senha na requisição de Login
- Remover cookie de login para evitar login automatico

## Service:

- No endpoint de cálculo do modelo matemático, atualmente ta salvando as métricas, salvando no banco, para o cálculo das medidas e assim para todo modelo matemático. Isso torna inconsistente a release minor quando dá algum erro no cálculo das outras hierarquias, pois já fez inserção. Além disso para métricas que precisam de mais de um valor, pega todas as salvar no intervalo de 20min. Mudar isso para pegar métricas recebidas pela action, fazer os cálculos e depois salvar todas as entidades;
- Mudar estrutura do services para separar pasta de produto e repositório de organização;
- Ajustar quantidade de características planejadas e realizadas no endoint de análise da release para o gráfico de release;

## CLI:

- Melhorar legibilidade/contraste de texto na CLI para diferentes tipos de cores de fundo do terminal
- Estudar possíveis melhorias na utilização dos arquivos .msgram e .metrics no fluxo
