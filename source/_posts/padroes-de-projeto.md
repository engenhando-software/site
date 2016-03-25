title: "Padrões de Projeto"
date: 2015-06-14T14:29:00.000-03:00
updated: 2015-09-07T21:30:13.729-03:00
tags: 
- "disciplina3"
- "modulo2"
- "unidade4"
permalink: "padroes-de-projeto"
comments: true
---

Privilegia principalmente a reutilização  

> Padrão de projeto é uma solução padronizada para um problema que se repete muitas vezes dentro de um determinado contexto.

## Padrões de criação

Diz respeito a padronizar a forma como os objetos são criados, compostos e representados.

### Abstract Factory

Prover uma interface para criação de famílias de objetos relacionados ou independentes sem que se especifiquem suas classes concretas.

### Factory Method

São métodos que retornam um novo objeto

### Singleton

Obter somente uma instância de um objeto na aplicação.

### Prototype

Quero que, dados dois objetos, eles sejam idênticos, mas não sejam a mesma instância.a1 = a2 não funciona porque eles viram a mesma instância.O Java já possui o método clone() que faz isso.

## Padrões Estruturais

Estão relacionados a como classes e objetos são compostos de forma a gerar estruturas maiores e mais complexas.

### Adapter

Com o adapter é possível por exemplo, trocar de uma biblioteca gráfica por outra sem grande impacto na aplicação.Definir uma interface que a aplicação (cliente) vai usar, implementar essa interface e dentro da implementação chamar os métodos da biblioteca gráfica. Ex. adaptada.desenharBotao();

### Flyweight

Dado um conjunto de pequenos objetos que possuem um atributo em comum, se cria apenas um objeto e todos os pequenos objetos apontam para o mesmo, economizando espaço em memória.  

### Proxy

Proxy representa uma visão diferente do objeto em questão. Por exemplo, um objeto representa uma imagem de satélite com alta resolução, cria-se o proxy desse objeto com a imagem de baixa resolução e posso manipular os dois da mesma forma, só que um é mais leve.  

### Façade

Dado que a aplicação precisa chamar a mesma sequencia de métodos em diversos locais diferentes, cria-se um Façade que faz essas chamas para aplicação e a aplicação só chama o Façade.  

### Composite

Representa estrutura de árvore. Um objeto pode ter nós que são da mesma interface Composite ou então ser uma folha.  

## Padrões Comportamentais

Estão relacionados ao comportamento dos objetos

### Chain of Responsability

Uma vez que existe uma cadeia de objetos, e é necessário ser enviado uma mensagem para um desses objetos. Esses objetos vão encaminhando para o próximo objeto da sequência até que um objeto identifique que a mensagem é pra ele. É uma lista encadeada.
