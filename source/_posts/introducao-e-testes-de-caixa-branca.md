title: "Introdução e Testes de Caixa-Branca"
date: 2015-08-10T21:52:00.000-03:00
updated: 2015-12-06T11:45:45.846-02:00
tags: 
- "disciplina1"
- "modulo3"
- "unidade1"
permalink: "introducao-e-testes-de-caixa-branca"
comments: true
---

O objetivo principal de qualquer técnica de testes é maximizar a relação percentagem de defeito sobre o número de testes feitos. O ideal é fazer o menor número de teste e testar a maior parte do sistema todo.  

### Princípios

*   Testar completamente é impossível
*   Testar é um trabalho criativo e difícil
*   Testes devem ser planejados e projetados
*   Teste requer independência (sem vícios)

### Conceitos

*   Casos de teste: conjunto de entradas possíveis do programa
*   Métodos de teste: métodos para se gerar casos de teste

*   Caixa branca ou estruturais
*   Caixa preta

### Métodos de Testes de Caixa Branca

#### Cobertura Lógica

São critérios que devem ser obedecidos para determinar os casos de testes.

#### Fatores para escolha dos critérios:

*   Complexidade do programa a se testar
*   Estrutura do programa a ser testado
*   Criticidade do programa a se testar
*   Nível de confiança que se deseja atingir

#### Critérios

*   Cobertura de comandos

*   Todos os comandos que existem no programa a ser testado sejam executados

*   Cobertura de decisões

*   O teste deve passar por todas as decisões do programa nos dois casos (verdadeiro e falso) pelo menos uma vez.

*   Cobertura de decisões-condições
*   Cobertura de múltiplas condições

*   Combinar todas as possibilidades nas duas decisões dadas no exemplo.

#### Método dos caminhos básicos

*   Fortemente embasado na teoria de grafos
*   Os casos de testes gerados passem por um número ótimo de caminhos entre a entrada e saída do programa

#### Definições

*   **Grafo de controle**: descreve o fluxo do programa
*   **Caminhos independentes**: é um caminho que não é constituído pela combinação de dois ou mais outros (não apresenta redundância).

*   Existem 3 formas de se contar o número de caminhos independentes (Complexidade Ciclomática)

*   Número de regiões: contar o número de regiões (blocos dentro do IF) e uma externa
*   C = E -N +2 onde, C número de caminhos independentes, E número de arestas e N número de nós.
*   Número de estruturas de decisão + 1

#### Geração dos casos de teste

Cada caminho independente gera um caso de teste
