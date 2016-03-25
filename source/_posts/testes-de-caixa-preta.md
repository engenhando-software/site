title: "Testes de Caixa-Preta"
date: 2015-08-14T23:13:00.001-03:00
updated: 2015-12-06T16:18:24.325-02:00
tags: 
- "disciplina1"
- "modulo3"
- "unidade2"
permalink: "testes-de-caixa-preta"
comments: true
---

3 métodos para geração de testes de caixa  

## Método 1: Partição de Classes de Equivalência

São casos de testes baseado na geração de valores típicos da entrada do programa.  

### Classe de Equivalência

É um subconjunto das entradas possíveis do programa

### Passos do método:

1.  Definir as condições de entrada

*   Faixa de Valores: 1 < ITEM < 1000
*   Conjunto ordenado: vetor de até 6 elementos
*   Conjunto de Valores: Enum
*   Condição booleana

3.  Definir as classes de equivalência: conjunto de valores que se entra no programa

*   Classe válida: 1 < ITEM < 1000
*   Classe inválida: ITEM <= 1 e ITEM >= 1000
*   As classes são divididas de acordo com o número de condições do programa

5.  Identificação dos casos de teste

*   Enumerar as classes de equivalência
*   Fazer os casos de teste para as classes válidas, as vezes com poucos casos de teste já possível englobar um número grande de classes válidas. 
*   Fazer os casos de teste para as classes inválidas, se for o caso, um caso de teste para cada classe inválida.

## Método 2: Grafo de Causa e Efeito

É baseado na análise das entradas do programa e saídas possíveis. A diferença do primeiro é que são todas formatadas para um formato booleano.Seja um programa simples que recebe dois tokens, as entradas possíveis são

1.  Primeiro token MOVTOX
2.  Primeiro token MOVTOY
3.  Segundo token é a letra de A a Z

Efeitos identificados70-Comando correto71-Mensagem M1 (msg de erro significa não é o token MOVTOX ou MOVTOY)72-Mensagem M2 (msg de erro significa não de token de A a Z

## Método 3: Análise de valores de fronteira

Trabalha especificamente com os valores que estejam próximos aos intervalos de validade de entrada do programa. Testa valores focados nas fronteiras dos intervalos.Princípio da Timidez: os bugs se encontram escondidos nos detalhes do programa.Ex.: Se os extremos da faixa são os valores a e b, geramos os seguintes casos de teste:

*   Entrada sobre a (sobre a fronteira inferior)
*   Entrada sobre  a - um valor bem pequeno (um pouco abaixo da fronteira inferior)
*   Entrada sobre b (sobre a fronteira superior)
*   Entrada sobre b + um valor bem pequeno (um pouco acima da fronteira superior)
