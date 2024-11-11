---
sidebar_position: 2
---

# Dashboards

## Mapa de Calor
Grafico que exibe a frequencia de uso semanal por hora das lojas

### Comando
```
yarn test -t heatMap
```

### Endpoint
```
/v1/billings/grouped/weekday
```
- `referenceDate`: Data de referencia para realizar a operacao de agrupamento;
- `granularity`: Referencia para agrupamento dos dados;

### Cenarios

- Garantir que retorna um valor maior que zero em operacoes no sabado;
- Garantir que retorna um valor maior que 105 em vendas ao meio-dia;
- Garantir que retorna um valor maior que 3 em operacoes totais ao ativar a granularidade diaria;

## Linha do Tempo
Todos os demais graficos do modulo de Dashboars referente a mudanca de granularidade

### Comando
```
yarn test -t timeTravel
```

### Endpoint
```
/v1/dashboard
```
- `referenceDate`: Data de referencia para realizar a operacao de agrupamento;
- `granularity`: Referencia para agrupamento dos dados;
- `limit`: Referencia para a paginacao;

### Cenarios

- "salesFollowUp" Garantir que o retorno lista um total diario e semanal como 9000 e o valor mensal como 9500;
- "paymentMethods" Garantir que o retorno possui um total de vendas com cartao de credito de 9500 na granularidade diaria;
- "paymentMethods" Garantir que o retorno possui um total de vendas com cartao de credito de 10500.52 na granularidade mensal;
- "machineOperations" Garantir que o retorno possui um total de ciclos de lavagens e secagens igual a 3 na granularidade diaria;
- "machineOperations" Garantir que o retorno possui um total de ciclos de lavagens e secagens igual a 4 na granularidade mensal;
- "cyclesOperations" Garantir que o retorno possui a primeira maquina com ciclos totais de 2; 
 