title: "Modelagem Arquitetural"
date: 2015-10-04T12:29:00.000-03:00
updated: 2015-12-05T19:07:30.790-02:00
tags: 
- "disciplina2"
- "modulo3"
- "unidade4"
permalink: "modelagem-arquitetural"
comments: true
---

Modelagem Arquitetural com modelo de visualização 4+1\. O objetivo é permitir que arquitetos possam capturar, comunicar e expressar de uma forma simples e visual como arquitetura foi pensada para seus times.  

*   Visualização lógica - perspectiva do usuário final e representa os grandes blocos de construção de um software, os pacotes.
*   Visualização de implementação - perspectiva para os desenvolvedores através de diagramas e componentes da UML
*   Visualização do implantação - topologia física, descrita através do diagrama de implantação.

## Visualização Lógica

Objetivo é capturar os principais elementos/módulo de um sistema e como estão relacionados.

### Diagrama de pacote

O objetivo é exprimir como dois ou mais pacotes se comunicam ou dependem um do outro. 

*   Dependência entre pacotes (linha pontilhada e seta aberta)
*   Um pacote dentro do outro - todo/parte 
*   O diagrama de pacotes permite expressar não só a decomposição funcional de um sistema como também padrões arquiteturais, p.ex. MVC.
*   É possível expressar também uma arquitetura n-camadas.

## Visualização de Implementação

*   Expressa os componentes de uma aplicação
*   Componentes são DLLs, libs, archives, assembly, JARs, WARs que constituem fisicamente uma aplicação

### Diagrama de componentes

*   Um componente na UML2 é uma classe estereotipada: <<component>>
*   Um componente pode representar qualquer tipo de software como ex. um banco de dados, um servidor de aplicação, servidor web, DLL, JAR
*   Dependência é igual aos pacotes (linha pontilhada e seta aberta)
*   Através da ligação interface requerida e interface fornecida é possível expressar mais informações no diagrama, do que somente dependência. Ex. browser tem uma interface requerida HTTP e IIS tem uma interface fornecida HTTP.
*   Quadrado no componente é chamado "porto"

## Visualização de Implantação

Permite expressar a visão topológica, implantação ou rede de um projeto. Representa como um software vai ser instalado e manifestado dentro máquinas na rede onde será hospedado e acessado pelos usuários.

*   Tem um caráter físico topológico, por isso fala de uma linguagem mais próxima da linguagem de produção, da infra.
*   Permite expressar elementos de hardware, processadores, dispositivos e redes de comunicação.
*   Permite mostrar onde os componentes vão residir.

### "Nodo" como elemento básico

*   É sempre um retângulo em 3D
*   Representa um elemento físico, um hardware com capacidade de processamento, ex: iPhone 5S, Samsung Galaxy Tab 3, ATM, Servidor de Banco de Dados
*   No diagrama a associação é representada como uma linha contínua
*   Dentro de um Nodo, podemos ter vários componentes com dependência, etc.
