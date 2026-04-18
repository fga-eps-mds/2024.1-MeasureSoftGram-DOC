# Plano de Custos

Planilha de custos do projeto disponível em: [Custos do MeasureSoftGram](https://docs.google.com/spreadsheets/d/1vEGKl1ZxSeijZwuVfzDAaH6eT9NllpKnPJGDVQK7TP0/edit?usp=sharing)

<iframe
src="https://docs.google.com/spreadsheets/d/1vEGKl1ZxSeijZwuVfzDAaH6eT9NllpKnPJGDVQK7TP0/edit?usp=sharing"
width="200%"
height="900">
</iframe>

<center>

<p>Documento 1 - Custos de desenvolvimento do MeasureSoftGram</p>

</center>


## Custo da Infraestrutura

### Deploy

<div align="justify">&emsp;&emsp;
O custo do deploy foi estimado a partir do valor do serviço de hospedagem em nuvem da Hostinger, um VPS (Virtual Private Server) com:
</div>

* 1 vCPU
* 50GB de espaço em disco NVMe
* 4GB de RAM


<div align="justify">&emsp;&emsp;
Isso é o mais próximo da infraestrutura necessária para o projeto inteiro, incluindo todos os microsserviços com custo de R$29,99 por mês. Além disso, foi acrescentado um adicional de R$16,99 por mês a fim de garantir o backup automático dos dados, o que é essencial para a segurança do projeto. Sendo assim, o custo semanal (por sprint) do deploy é de R$16,33.
</div>

### Domínio

<div align="justify">&emsp;&emsp;
Custo fixo de R$ 49,90 para o registro do domínio "measuresoftgram.com.br" por um ano, valor encontrado no site da Hostinger.
</div>

### Depreciação do Computador

<div align="justify">&emsp;&emsp;
O custo semanal do computador foi calculado com base na depreciação linear do equipamento. Foi utilizado como referência um notebook Acer Aspire 5 (AMD Ryzen 5, 16GB RAM, 512GB SSD), com valor de R$ 3.665,56, e vida útil estimada de 60 meses (aproximadamente 257 semanas), resultando em uma depreciação semanal de R$ 14,26 por máquina.
</div>

## Custo de Energia e Internet

<div align="justify">&emsp;&emsp;
Os custos de energia elétrica e internet foram calculados com base no consumo semanal estimado durante o desenvolvimento remoto. Para a energia, considerou-se a tarifa vigente da Neoenergia Brasília (R$ 0,83/kWh) e um consumo médio de 35–40W para o computador e 8–12W para o modem. Para a internet, foi utilizado como referência um plano de 600 Mega da Claro, com valor médio de R$ 99,90/mês (R$ 23,31/semana).
</div>

| Item                               | Consumo por hora | Custo por semana |
|------------------------------------|------------------|------------------|
| Computador (energia)               | R$ 0,03          | R$ 0,41          |
| Modem (energia)                    | R$ 0,01          | R$ 0,12          |
| Internet                           | -                | R$ 23,31         |
| **Total (remoto por semana)**      | -                | **R$ 23,83**     |

<center>

<p>Tabela 1 - Custos de Energia e Internet</p>

</center>

## Custo por Membro

<div align="justify">&emsp;&emsp;
O custo semanal por membro foi calculado somando o custo presencial na Universidade de Brasília (UnB) com o custo de desenvolvimento remoto. O custo por hora na UnB foi estimado em R$ 58,37, com base no custo médio anual por aluno em universidades federais de R$ 52.533,00 e uma carga horária anual de aproximadamente 900 horas cursadas. Considerando 14 horas semanais de atividades presenciais e 18 horas remotas, o custo total semanal por integrante é de R$ 257,31.
</div>

| Descrição                         | Valor por semana |
|-----------------------------------|------------------|
| Custo presencial (UnB)            | R$ 233,48        |
| Custo remoto (energia + internet) | R$ 23,83         |
| **Custo total por membro**        | **R$ 257,31**    |

<center>

<p>Tabela 2 - Custo por Membro</p>

</center>

> Não foi acrescentado o custo da mão de obra.


## Histórico de Versão

| Versao | Data       | Descricao            | Autor                                    | Revisor |
|--------|------------|----------------------|------------------------------------------|---------|
| 1.0    | 18/04/2026 | Criação do documento | [João Antonio](https://github.com/i-JSS) |         |