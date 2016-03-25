title: "Projeto Comportamental"
date: 2015-05-16T14:23:00.000-03:00
updated: 2015-09-05T15:17:30.261-03:00
tags: 
- "disciplina2"
- "modulo2"
- "unidade2"
permalink: "projeto-comportamental"
comments: true
---

## Contrato de Operações

*   Ajudam a definir o comportamento do sistema, descrevendo o resultado das execuções das operações do sistema
*   Objetos de domínio: as classes dão origem aos objetos do sistema, os objetos mudam de estado.

### Seções de um contrato

*   Operação: nome e parâmetros da operação
*   Referências cruzadas: casos de uso nos quais esta operação deve ocorrer
*   Pré-condição: hipóteses dignas de nota sobre o estado do sistema. Essas hipóteses não serão testadas na lógica da operação.
*   Pós-condição: o estado dos objetos no modelo de domínio, concluída a operação. <span style="background-color: yellow;">É importante descrever na mudança de estado: criação ou remoção de instância, criação ou exclusão de associação, alteração de atributo.</span>

> Descrever o resultado sem se importar "como".

Quando usar contratos  

*   É importante utilizar contratos quando existem muitos objetos de domínio que estão sendo criados, modificados, etc. num único passo do caso de uso. 
*   É útil usar contratos também quando não é claro quais objetos serão atualizados pela descrição dos casos de uso.
*   Não é necessário fazer contratos para toda operação do sistema, em geral, só o caso de uso basta.

Para fazer contratos

*   Identifique operações de sistema a partir dos <span style="background-color: yellow;">diagramas de sequência</span> de sistema.
*   Para operações do sistema que são complexas
*   Para descrever as pós condições, use as seguintes categorias:

*   Criação e remoção de instância
*   Modificação de atributo
*   Associação formadas e desfeitas

## Responsabilidades, princípios e padrões de projeto

Responsabilidade é um contrato que uma classe tem. Existem dois tipos de responsabilidade:  

1.  Conhecer dados privados. São derivadas dos atributos dos objetos 
2.  Fazer: criar objetos, realizar cálculo, etc. São derivadas dos métodos.

Responsabilidade pode envolver um ou mais métodos de um ou mais objetos.Interações são trocas de mensagem entre objetos no sistema, e quando se troca mensagens estamos atribuindo responsabilidades a um objeto, já que ocorre a interação de um objeto com outro.  

### Padrões de Projeto

Padrões de desenvolvimento: expressam uma solução para um determinado problema em um determinado contexto.  

Padrões arquiteturais: expressam uma solução num nível mais alto de abstração.  

Exemplos de padrão arquitetural:  

*   Modelo visão-controle: MVC
*   Camadas: só se comunica com as camadas adjacentes
*   Padrões GRASP

*   Controlador
*   Coesão alta
*   Acoplamento baixo
*   Polimorfismo

*   Padrões de domínio: o principal foco deve ser o domínio, a logica do domínio.

*   Entidades
*   Objetos de valor
*   Serviços
*   Fábricas

### Princípios de projeto

Representam um conjunto de diretrizes que ajudam a evitar que um projeto fiquei ruim ou de baixa qualidade. Deve ser evitado nos projetos:

*   **Rigidez:** sistema muito acoplado
*   **Fragilidade**: uma parte para de funcionar quando se faz alteração em outra parte não relacionada.
*   **Imobilidade**: muito difícil ou arriscado separar uma parte da aplicação para ser usada em outro projeto.
*   **Viscosidade**: fazer coisas corretas é mais difícil do que fazer coisas erradas.
*   **Complexidade** desnecessária
*   **Repetição desnecessária**: projeto possui estruturas repetidas que não podem ser unificadas.
*   **Opacidade**: intenção do projeto não está bem expressada.

Deve-se procurar praticar:

*   Única responsabilidade
*   Manter o controller simples e a lógica deve ficar no domínio 
*   Restringir as associações ao máximo, torna o projeto mais claro

## Responsabilidades, interações e realizações de casos de uso

Mensagens são utilizadas com objetivo de cumprir as responsabilidades. Uma mensagem indica uma operação existente no objeto receptor.  

### Construindo diagramas de interação

A maioria dos objetos envolvidos nesse diagrama já foram identificados no diagrama de classe de domínio. Diagrama de interação vai estar consistente com os casos de uso e as classes de domínio.  

No ciclo de vida iterativo/incremental os modelos vão evoluindo, então:  

Modelo de classes serve como base para o modelo de interações  
Mod. Interações ajuda o refinamento do modelo de casos de uso  
Mod. Interações ajuda gerar operações para o modelo de classes  
Mod. Interações gera novos atributos para o modelo de classes  

Exemplo de diagramas de interação de um PDV  

## Diagrama de Classes de Projeto

Classes de projeto ilustram as especificações para as classes de software e interfaces.  
Acontece em paralelo ao diagrama de interação  

### Criando classes de projeto

*   Identificar as classes que fazem parte do diagrama;
*   Acrescentar atributos identificados no modelo de domínio;
*   Acrescentar operações (analisando o diagrama de interação);

### Visibilidade entre objetos

É a habilidade de um objeto ver ou ter referência a outro objeto.  

*   Visibilidade por atributo

*   Existe de A pra B quando B é um atributo de A

*   Visibilidade por parâmetro

*   Existe de A pra B quando B é passado como parâmetro para um método de A

*   Visibilidade local

*   Existe quando B é declarado como um objeto local dentro de um método de A

*   Visibilidade global

*   Existe quando B é declarado como um objeto global em A

> **Navegabilidade** é a propriedade do papel que indica que é possível navegar unidirecionalmente por meio da associação de objetos da classe de origem para objetos da classe alvo. (Seta nos diagramas de classe para ligar duas classes)

## Diagrama de transição de estados 

Esses diagramas são uma complementação para modelagem comportamental.  

### Estado

*   **Estado** é uma situação na vida de um objeto em determinado momento no tempo em que ele satisfaz a alguma condição ou realiza alguma atividade.
*   Cada estado é determinado pelos valores dos atributos ou pela ligações com outros objetos.
*   Em geral, possui um único estado inicial pode ou não possuir estados finais.

### Evento

*   Uma transição possui um evento associado
*   Um evento é algo que acontece em algum ponto do tempo e que pode modificar o estado de um objeto. Ex. Pedido Realizado, Fatura paga, Cheque devolvido, etc.
*   Condição de Guarda é uma espécie de "If" que valida se a transição vai ocorrer quando for disparada por um evento.

### Ações

*   Ações são tudo que um objeto realiza quando transita de um estado para outro.
*   É expressa em termos de atributos, operações, associações da classe, etc. 
*   Está associada sempre a uma transição. E é executada somente se uma transição for disparada.

### Objetos dependentes de estado

> Os diagramas de estado devem ser criados para objetos dependentes de estados, ou seja, objetos que reagem diferente dependendo de seu estado.

### Tipos

Existem dois tipos de objetos dependentes de estado:

*   **Objetos Reativos**: 

*   Complexos: telefone, carro, microondas, elevador
*   Transações ou objetos de negócio: venda, pedido, pagamento reagem a eventos como cancelar, adiar, faturar, etc.
*   Protocolos de comunicação
*   Fluxos de navegação de pagina, janela, menu, interface com usuário
*   Controlador de sessão de um fluxo de interface em páginas web, guarda o estado da sessão no cliente web e dependendo desse estado ele reage diferente.

*   **Sequências de operações**: as operações que chegam ao sistema tem que chegar numa determinada ordem de estados. Para definir essa ordem, usamos o diagrama de estados. Ex. Estados: EsperandoPorVenda -> EntrandoItens -> EsperandoPagamento -> AutorizandoPagamento.
