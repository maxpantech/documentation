---
sidebar_position: 1
---

# Introducao

### O que sao testes de integracao?

Sao testes que visam unir dados mockados com a logica por tras do servico, sao mais utilizados no backEnd, principalmente visando retornos corretos dentros das rotas quando as mesmas dependem de banco para realizar a entraga!

### Quando criar?

O ideal e mais correto seria desenvolver primeiro os testes de respostas esperadar quando for iniciar uma feature no back, assim voce pode usar os testes como garantia que sua feature esta respondendo como deveria, sem precisar subir a aplicacao inteira localmente a todo momento, pois nos testes voce ira mockar dados no banco fake e usar padronizar suas respostas a partir desse mock.

![Docs Version Dropdown](./imgs/tdd.png)