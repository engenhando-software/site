title: "Visão Geral da Arquitetura de Software"
date: 2015-09-03T22:01:00.000-03:00
updated: 2015-09-03T22:01:02.936-03:00
tags: 
- "disciplina2"
- "modulo3"
- "unidade1"
permalink: "visao-geral-da-arquitetura-de-software"
comments: true
---

## Exemplo prático de arquitetura de software

Antes de aplicar a arquitetura de software para resolver um problema, deve analisar os condutores para se chegar nas soluções dos problemas desses condutores.

## O que é uma arquitetura de software

> "Arquitetura de software é o conjunto de decisões que, se feitas incorretamente, podem causar o cancelamento do projeto" - Eoin Woods

Tipos de arquitetos  

*   Arquiteto de soluções

*   Responsável por trabalhar com times comercial e pré-venda na solução pré-liminar de um projeto. 
*   Antes do projeto ser aprovado. 
*   Faz a ponte entre outros arquitetos, em particular do arquiteto de software.

*   Arquiteto de software

*   Papel central: liderar a construção de uma arquitetura desde o primeiro dia do projeto
*   Usa-se os requisitos críticos
*   Toma decisões técnicas

*   Arquiteto de dados

*   Desafios como BI, ETL, etc.
*   Tomada de desciões técnicas

*   Arquiteto de Infraestrutura

*   Ex.: computação nas nuvens

*   Arquiteto de tecnologia Java EE
*   Arquiteto de tecnologia .NET
*   Arquiteto das nuvens

### Conceitos sobre o arquiteto de software

*   O arquiteto é um desenvolvedor sênior

*   Falso
*   Enquanto o desenvolvedor é um especialista, o arquiteto é um generalista.
*   O arquiteto **não** é um desenvolvedor sênior

*   O arquiteto domina as APIs de segurança Java ou .NET

*   Falso
*   Mas precisa dominar as táticas e soluções de mercado que ele vai trabalhar
*   O arquiteto domina as **táticas arquiteturais** de segurança

*   O arquiteto desenha plantas e o time de desenvolvimento implementa

*   Falso
*   O arquiteto <span style="background-color: yellow;">junto</span> com o time de desenvolvimento desenvolve cria plantas

*   O arquiteto desenvolve a arquitetura

*   Falso
*   Ele desenvolve a arquitetura <span style="background-color: yellow;">junto</span> com time
*   O time de arquitetura desenvolve a arquitetura

### O que faz um arquiteto de software

> Liderar a concepção do software...  
> ...Definindo os atributos de qualidade.

> Fornece apoio à construção do software...  
> ...Baseado nos atributos de qualidade.

### Decomposição típica das atividades de um arquiteto

*   Coleta de requisitos (25%)
*   Modelagem e implementação de provas de conceito (50%)

*   Provas de conceitos são instrumentos para que arquitetos possam reduzir riscos

*   Assistência ao time (25%)

## O contexto na arquitetura de software

*   É preciso olhar o contexto ambiental onde o arquiteto está envolvido para se tomar decisões arquiteturais. Ex. mudar de framework quando não se tem tempo, nem experiência.

### Influências na arquitetura

*   Contexto de negócio

*   Qual a natureza do projeto que se está trabalhando? Se está trabalhado com um projeto de tempo fechado, não se pode ofender o prazo.

*   Diretrizes e requisitos

*   Captar as diretrizes do projeto como  escalabilidade, segurança, usabilidade que são elementos críticos.

*   Restrições e premissas 

*   Tempo, custo e muitas outras restrições. Ex. time júnior sem capacitação.

*   Experiência do time

*   Ignorar a experiência do time pode trazer consequencias graves no projeto.

*   Soluções técnicas disponíveis

*   São chamados de ativos arquiteturas. Podem ser elementos importantes para guia o arquiteto no caminho de boas soluções técnicas.

*   Atributos de qualidade diversos

*   Aspectos como segurança da informação, performance, usabilidade. É preciso conhecer esses atributos para se alcançar uma boa arquitetura

## Decisões arquiteturais

> "A vida de um arquiteto de software é uma longa sucessão de decisões sub-ótimas e parcialmente tomadas no escuro." - Philippe Kruchten

### Pontos a serem observados ao tomar decisões

*   Alinhamento estratégico

*   nunca colocar a tecnologia na frente do negócio.

*   Balanceamento de influências diversas

*   experiência do time
*   ativos da empresa
*   contexto de negócio (diretrizes)

*   Análise de riscos
*   Processo decisório

*   O que é melhor para o projeto e não o que o desenvolvedor quer fazer.
