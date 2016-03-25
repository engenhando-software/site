title: "Conceitos de Programação Orientada a Objetos"
date: 2015-05-24T18:45:00.000-03:00
updated: 2015-08-15T22:11:09.207-03:00
tags: 
- "disciplina3"
- "modulo2"
- "unidade1"
permalink: "conceitos-de-programacao-orientada-a-objetos"
comments: true
---

### Conceitos Básicos de OO (cap. 1)

*   Classes consistem na descrição de atributos e métodos para um conjunto de objetos. Possuem uma visão interna e externa (funções publicas).
*   Interface pública são os serviços da classe que poderão ser utilizados por outras partes do programa, ocultando como os serviços são implementados. Essa ocultação é chamada **encapsulamento**.
*   Objetos são entidades unicamente identificados. Eles são uma instancia concreta e dinâmica de uma classe. Possuem dados, comportamento e identidade da classe. Pode-se dizer que um objeto é "uma variável do tipo de dados definido pela classe".
*   Os métodos de uma classe podem ser chamados de funções membros ou serviços.
*   O estado de um objeto é determinado pelo valor de seus atributos
*   Modificadores de acesso

*   Público - visíveis em toda aplicação
*   Privado - visíveis apenas internamente a classe que foram programados
*   Protegido - visibilidade intermediária, visíveis apenas em uma hierarquia de classes (subclasses)

*   Herança

*   Criar classe mãe e classes filhas que especializam um determinado comportamento
*   Herança múltipla: duas ou mais classes que possuem subclasses (java e c# não implementa esse conceito)

### Linguagem Java - (cap. 3)

*   Em java, um objeto é interpretado como uma referência e não o objeto propriamente dito.
*   NomeClasse nomeObjeto -> cria-se referência mas não objeto; uma vez criado objeto com "new" a referência não pode ser manipulada numericamente.
*   Construtor: iniciam o objeto
*   Modificador "friendly" - visíveis apenas no mesmo pacote
*   Membros estáticos: os atributos declarados como estáticos, possuem o mesmo valor durante a execução.
*   Destrutores: são utilizados para finalizar um objeto.

### Herança de Classe (cap. 4)

*   Extends
*   Atributos protegidos podem ser explicados depois que o conceito de herança de classe foi introduzido

*   Membros protegidos podem ser acessados por classes do mesmo pacote mesmo que não sejam da mesma hierarquia de classes
*   Podem ser acessados por classes que estendem dessa classe, mesmo que esta subclasse seja de outro pacote
*   Membros protegidos se limitam a uma hierarquia de classes, uma vez que java não permite herança múltipla de classes
*   Membros protegidos e estáticos podem ser acessados em qualquer classe estendida

*   Construtores em classes estendidas

*   Quando uma subclasse é construída, uma superclasse também é.
*   A nova classe (derivada) deverá escolher qual construtor da superclasse deseja chamar
*   Subclasse chama o construtor da superclasse através do super() com a mesma assinatura da superclasse

### Polimorfismo (cap 5)

*   Reescrever métodos com mesmo nome, parâmetros diferentes, etc.
*   Palavra chave super, pode-se usar super.metodo()
*   Palavra chave final, serve para definir atributos ou métodos que não podem ser modificados após sua primeira inicialização.
