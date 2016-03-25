title: "Arquitetura Orientada ao Modelo (Model Driven Architecture-MDA)"
date: 2015-06-03T22:22:00.002-03:00
updated: 2015-09-07T20:24:38.007-03:00
tags: 
- "disciplina3"
- "modulo2"
- "unidade3"
permalink: "arquitetura-orientada-ao-modelo-model-driven-architecture-mda"
comments: true
---

## Arquitetura Orientada Ao Modelo

*   Foi um paradigma criado pelo OMG em 2000
*   Ciclo de vida é semelhante ao tradicional, cria-se os mesmos modelos das abordagens tradicionais.
*   A ideia é iniciar um projeto de modelagem que vai ser num primeiro momento independente de plataforma, chamado:

*   **PIM - Platform Independent Model**
*   Logo depois, 
*   **PSM - Platform Specific Model**
*   E depois será convertido em código fonte.

Dentro do conceito de MDA, surge também o MOF - Meta Object Facility, que é uma instância do conceito de MDA.

> MOF define uma linguagem abstrata e um framework para especificação, construção e gerenciamento de metamodelo. A UML implementa o MOF.

### Tabela do MOF

*   M3 - Nível mais alto de abstração. É a especificação de conceitos do modelo MOF
*   M2 - Nível de implementação de linguagens como UML
*   M1 - Mais comum. Onde os modelos são criados. 
*   M0 - Nível das instancias que são criadas a partir desse modelo. Se temos uma tabela Produto, o nível M0 seria os registros dessa tabela.

XMI é uma especificação genérica que é possível exportar diagramas entre softwares diferentes (Argo e Rational)

## EMF - Eclipse Modeling Framework

*   É um framework que é utilizado para geração de aplicações dentro do conceito de MDA.
*   Base para trabalhar com EMF é um doc XMI, Rational, java anotado, etc.
*   É semelhante ao MOF mas definição é chamada "EMOF".

Constituído de dois frameworks fundamentais:  

*   Core Framework: suporte para criação de classes de implementação
*   EMF.edit: suporte para edição do modelo
