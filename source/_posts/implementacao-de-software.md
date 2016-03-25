title: "Implementação de software"
date: 2015-05-26T21:09:00.000-03:00
updated: 2015-09-07T19:59:58.566-03:00
tags: 
- "disciplina3"
- "modulo2"
- "unidade2"
permalink: "implementacao-de-software"
comments: true
---

## Frameworks

É com a experiência dos programadores que foram surgindo os frameworksConstruir um software do zero é muito custoso, por isso se usa uma base já implementada

### Benefícios de se usar um framework

*   O benefício básico de se usar um framework é a produtividade
*   Melhora da qualidade através da reutilização do framework, já que ele é mais usado e se detecta mais falhas

Com restrições de prazo e custo, os desenvolvedores devem-se utilizar de componentes, frameworks e padrões de projeto para realização do projeto

### Definições

Framework é uma técnica que se beneficia de três características das linguagens de programação orientadas a objeto: abstração de dados, poliformismo e herança; O framework é uma arquitetura semi-acabada e passível de reutilização para um domínio de aplicação;Framework é uma aplicação genérica que permite a criação de diferentes aplicações em um determinado domínio;Um framework define uma arquitetura para uma família de sistemas, fornecendo partes predefinidas para sua construção;

### Conceitos de Frozen Spots e Hot Spots

**Frozen Spots**: definem uma arquitetura global de um sistema que permanece **inalterado** em qualquer instanciação do framework;**Hot Spots**: são pontos do framework onde ocorrem a especialização (definir classes adicionais para sobrepor métodos, etc.) e adaptação.

### Esquema de HotSopts

*   Uma classe abstrata de base, que vai definir a interface
*   Classes concretas derivadas, representando cada uma das diferentes alternativas para os aspectos variáveis
*   Parte opcional com relacionamentos e classes adicionais

### Benefícios

*   Modulariação
*   Reutilização
*   Extensão de interfaces
*   Framework controla estrutura e abordagem do programa

### UML-F 

Usada para fazer modelagem de frameworks e utiliza conceitos comuns e mecanismos de extensão (como estereótipos) da própria UML.

*   Estereótipos

*   São mecanismos para permitir adicionar novos blocos de construção semelhantes aos existentes
*   É representado graficamente por << e >>

*   Tag values

*   São meios para proporcionar a criação de novas propriedades. É apresentado como uma sequencia de caracteres entre chaves, colocado abaixo de outro elemento.

*   Restrições

*   São mecanismos para especificar uma nova semântica de algum elemento UML. É representada como uma sequencia de caracteres colocada próxima ao elemento associado.

### Hot Spots

Há três tipos de hot spots em um framework orientado a objetos:

*   Métodos variáveis: possuem uma interface bem definida, mas que podem variar sua implementação de acordo com a instanciação do framework;
*   Classes estendidas: podem ser estendidas durante a instanciação do framework, recebendo novos métodos;
*   Interfaces estendidas ou classes abstratas: permitem a criação de subclasses concretas na instanciação do framework. Essas classes são chamadas de classes de aplicação.

Os três tipos podem ser estáticos (instanciação não é requerida em tempo de execução) ou dinâmicos (é requerida em tempo de execução)

### Tags utilizadas em UML-F

*   Variable: é aplicado aos métodos de uma classe e representa o hot spot Métodos Variáveis;
*   Extensible: é aplicada a uma classe e indica o hot spot Classes Estendidas. 
*   Incomplete: representa o hot spot Interfaces Estendidas. Colocada ao lado do simbolo de generalização;
*   Tag appl-class: Complementa a definição de classes estendidas. Indica um aditivo na estrutura de um framework;
*   static e dynamic: complementam a notação dos hot spots, indicando se o mesmo requer instanciação ou não.
