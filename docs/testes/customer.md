# Customers

## Credits
Validacoes na adicao e subtracao dos creditos do cliente;

### Comando
```
yarn test -t Credits
```

### Endpoint
```
/v1/orders
/v1/users/customer-stores?
```
- `documentId`: Cpf ou documento do cliente;
- `limit`: Referencia de paginacao;
- `page`: Referencia de paginacao;


### Cenarios

- Garantir que apos adicionar o credito ao cliente, a listagem de credito do mesmo seja atualizada;
- Garantir que apos remover o credito ao cliente, a listagem de credito do mesmo seja atualizada;
- Garantir que nao e possivel remover um credito maior do que a carteira do cliente, e que apos a tentativa a listagem nao seja alterada;
