# Machines

## Custom Prices
Precos personalizados para maquinas;

### Comando
```
yarn test -t CustomPrices
```

### Endpoint
```
/v1/machines/custom-price
/v1/stores/ID_DA_MAQUINA
```

### Cenarios

- Garantir que um preco customizado criado no momento atual substituira o preco normal;
- Garantir que um preco customizado criado para as proximas 24 horas NAO substituira o preco normal;
- Garantir que um preco customizado criado para uma hora a frente NAO substituira o preco normal;
- Garantir que um preco customizado criado em uma timezone diferente de -3 substituira o preco normal;
 