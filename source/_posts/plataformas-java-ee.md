title: "Plataformas Java EE"
date: 2015-10-19T22:07:00.001-02:00
updated: 2015-12-05T23:21:37.884-02:00
tags: 
- "disciplina3"
- "modulo3"
- "unidade2"
permalink: "plataformas-java-ee"
comments: true
---

## Tecnologias básicas de Java EE

### JSF

"A tecnologia Java Server Faces é um framework de componentes no lado servidor para interfaces de usuários Web baseada em tecnologia Java", Java EE 6 TutorialJSF é uma especificação, a implementação é o PrimeFaces, RichFaces, IceFaces.Cuida da renderização de páginas web. É multicamadas e multi-plataforma. 

### Servlets

"Um servlet é uma classe da linguagem Java que é usada para estender as capacidades de servidores que hospedam aplicações por meio de um modelo de programação requisição-resposta", Java EE 6 TutorialFaz a ligação entre a lógica de negócio e as páginas web. Faz roteamento, auditoria, transações

### JAX-WS

"Provê a funcionalidade para serviços Web grandes baseado nos protocolos comuns WS-*", Java EE 6 TutorialUsado para integração com outros sistemasÉ apenas uma especificação Apache CXF, JBOSS WebServices

### JAX-RS

"Provê a funcionalidade para serviços web no estilo RESTful", Java EE 6 TutorialÉ apenas uma especificação, um exemplo de implementação é o Apache Jersey

### JPA

"A API de persitência Java provê facilidades de mapeamento objeto relacional para gerenciar dados relacionais em aplicações Java", Java EE 6 Tutorial

## Tecnologias avançadas de Java EE

### EJB

É um componente servidor que encapsula a lógica de negócio de uma aplicação  
Adiciona poderes a uma classe e permite que a aplicação se torne muito escalável.  

#### Vantagens

*   Controle transacional automático
*   Capacidade de operar em ambientes distribuidos
*   Facilita a montagem do estilo arquitetural de microserviços ou implantações SOA (é comparável ao WCF nesse sentido) 

### JMS

É uma API Java que permite que aplicações criem, enviem, recebam ou leiam mensagensÉ uma especificação e pode ser comparado ao MQServices da IBM ou MSMQ da Microsoft.Implementação dessa especificação é o Apache MQ

### JTA

Permite que aplicações acessem transações de uma maneira independente de implementações específicas.  
É um controle de transação global, por exemplo, fazer o controle da transação para enviar dados a receita e salvar esses dados no banco local. Nesse caso, não adianta fazer controle da transação somente no banco de dados.  

### JCA

A arquitetura de conectores Java EE permite que componentes Java EE interajam com sistemas legados. Ex. SAPCC.  
É uma alternativa mais avançada quando o JAX-WS ou JAX-RS não nos permite fazer a integração com sistemas legados.  

## Plataforma Java EE

É uma das principais plataformas para desenvolver Web e Distribuído. A plataforma Java EE pode ser representada por uma imagem:  

[![](http://docs.oracle.com/javaee/5/tutorial/doc/figures/overview-multitieredApplications.gif)](http://docs.oracle.com/javaee/5/tutorial/doc/figures/overview-multitieredApplications.gif)  

O Java EE é na verdade um conjunto de especificações coordenado por um conjunto de empresas, por isso, o Java EE não representa uma tecnologia específica.  

Os servidores de aplicação para o Java EE mais conhecidos são:  

*   Apache Tomcat
*   JBOSS Web Server
*   JBOSS Application Server
*   IBM WebSphere WebServer
*   IBM WebSphere Application Server
*   Oracle Application Server
