title: "Métricas e Estimativas de Projetos"
date: 2015-06-24T22:47:00.004-03:00
updated: 2015-09-06T15:22:21.353-03:00
tags: 
- "disciplina4"
- "modulo2"
- "unidade2"
permalink: "metricas-e-estimativas-de-projetos"
comments: true
---

## Métricas, Estimativas e Modelos de software 

### Qualidade

A avaliação da qualidade está relacionada a uma série de características intrínsecas do produto, ex.,  

*   Quantidade de bugs
*   Conformidade com requisitos
*   Desempenho
*   Indicador de qualidade

### Métrica

É a medição de atributos de um processo, projeto, etc. É também uma relação entre medidas.  

#### Atividades de medição e análise são importantes para:

*   Caracterizar ou permitir entender processos, produtos, recursos e ambiente.
*   Avaliar para determinar o status do projeto, com respeito aos planos feitos
*   Predizer valores observados possam ser utilizados para predizer outros
*   Melhorar, identificando causas de problemas e ineficiências e oportunidades de melhoria

#### Escalas de mensuração

*   Nominal: escala inicial, baseada em uma avaliação nominal
*   Ordinal: baseada numa ordem pre-estabelecida. Ex prioridade mínima, média, max.
*   Intervalar: baseada em intervalos. Ex temperatura
*   Razão: existe uma relação natural entre os valores. Ex: Salário
*   Nas métricas de software serão usadas basicamente as escalas de razão e ordinal

#### Algumas métricas conhecidas no desenvolvimento de software:

*   Números de linhas de código 
*   Número de pessoas para implementar um caso de uso
*   Número de defeitos encontrados num produto
*   Esforço necessário para realizar uma tarefa/projeto
*   Tempo necessário para realizar uma tarefa/projeto
*   Custo necessário para realizar uma tarefa/projeto
*   Grau de satisfação do cliente

#### Objetivos

*   Melhorar a previsibilidade e a chance de sucesso no projeto.
*   Permitir melhor gerenciamento do projeto
*   Reduzir pressões sobre cronogramas
*   Apoiar decisões make or buy fazer/comprar
*   Indicar a qualidade de um produto de software
*   Avaliar benefícios
*   Avaliar ROI

#### Características de uma boa métrica

*   Facilmente calculada, entendida e testada
*   Pode ser automatizável
*   Deve ser útil para de estudos estatísticos
*   Deve ser repetível, objetiva
*   Capaz de indicar um caminho de melhoria

#### <span style="background-color: yellow;">Classificação</span>

*   Métricas Diretas

*   É aquela que é realizada em termos <span style="background-color: yellow;">atributos observáveis</span>. Números de linhas, número de erros, etc

*   Métricas Indiretas

*   <span style="background-color: yellow;">São baseadas em medidas diretas</span>. Ex. facilidade de manutenção, produtividade, esforço, tamanho baseado em funcionalidade. Não são observáveis diretamente.

*   Métricas orientadas a tamanho

*   São aquelas aplicáveis a contagem de tamanho de artefatos de software. Ex.: KLOC, número da páginas de documentação.

*   Métricas orientadas à função

*   Se baseia em métodos para medição de software do ponto de vista do usuário. Ex. Ponto de função, ponto de caso de uso, etc.

### Análise de Pontos de Função (APF)

Consiste na contagem das funções que caracterizam um sistema, sob o ponto de vista do que ele faz para o usuário.

*   Mede a funcionalidade entregue ao cliente (métrica indireta)
*   Utiliza um método padronizado internacionalmente
*   Pode ser usada tanto no início, no meio ou no final do projeto de software
*   Útil para medição de produtos novos ou existentes, em evolução
*   É baseado em função de dois tipos. 

*   **Dado**: relacionam-se ao modelo de dados. Dividem-se em Arquivos Lógicos Internos (ALI) e Arquivos de Interface Externa (AIE)
*   **Transação**: estão relacionadas "as transações realizadas no escopo da aplicação. Geralmente são captadas por meio de casos de uso. Dividem-se em Entradas Externas (EE), Saídas Externas (SE) e Consultas Externas CE).

*   É uma métrica indireta e funcional.

#### O que deve ser contado num produto, segundo a APF?

1.  Entradas: transações que alteram o estado do sistema. Ex: CRUD
2.  Saídas: transações que enviam dados para fora do sistema. Ex: Arquivos de interface
3.  Consultas: transações de consulta a bases de dados
4.  Arquivos Lógicos Internos: arquivos mantidos pelo sistema
5.  Arquivos de Interface Externa: arquivos externos que não são mantidos pela aplicação

#### Tipo de Contagem de PF

*   **Contagem Indicativa**: feita no momento inicial do projeto com um modelo preliminar dos dados.
*   **Contagem Estimada**: realizada quando se possui detalhes suficientes para fazer uma estimativa melhor. Quando se tem um modelo de funções básicas.
*   **Contagem Detalhada**: bastante confiável, realizada quando se tem informações completas sobres as funções e dados.

#### Etapas do processo de contagem de pontos de função

1.  Identificação das funções do sistema
2.  Classificação de cada função de acordo com sua complexidade funcional
3.  Cálculo dos pontos de função brutos através de pesos de acordo com uma tabela
4.  Avaliação das 14 "características gerais" do sistema
5.  Determinação do fator de ajuste (específico do projeto)
6.  Cálculo dos pontos de função ajustados

#### Contagem por pontos de função

É feito por 5 etapas.

*   Entradas

*   São elementos que vão alterar algum estado dos dados na aplicação

*   Saídas

*   São funcionalidades que provem a troca de dados na saída de dados

*   Arquivos lógicos internos

*   São arquivos que armazenam informações da aplicação internamente

*   Arquivos de interface externo

*   São arquivos de outras aplicações que são apenas acessados

*   Consulta

*   Trazem dados que estão armazenados mediante uma seleção desses dados

#### Transações podem ser

*   Entrada 
*   Saída 
*   Consulta

A produtividade de uma equipe pode ser determinada com a quantidade de horas gastas para disponibilizar uma quantidade de pontos de função.  

> **Produtividade = Tamanho do Produto / Esforço**

Obs.: Tamanho do Produto pode ser em diversas unidades, como PF/HH, PF/PM.  

> **Esforço = Pessoas x Tempo**

Prdutividade média é baseada em dados históricos, com a fórmula:  

> **Qtd. Pessoas = Tamanho / (Produtividade x Tempo)**

#### Itens de influência (Fatores de Ajuste)

1.  Teleprocessamento
2.  Processamento Distribuído
3.  Performance
4.  Carga de Máquina
5.  Volume de Transações
6.  Entradas de dados online
7.  Atualizações online
8.  Eficiência do usuário final
9.  Complexiadade do processamento
10.  Reutilização de código
11.  Facilidade de implantação
12.  Facilidade de operação
13.  Facilidade de manutenção/alterações
14.  Operação em múltiplos locais

#### Etapas para o cálculo da produtividade

*   Medição do tamanho em pontos de função
*   Registros históricos para determinar o escopo (medido em homens x hora)
*   Calcular a produtividade obtida - Horas/PF ou PF/HH
*   Estabelecer as produtividades médias para os diversos ambientes de desenvolvimento e tipos de projeto

#### Fatores que influênciam na produtividade de um projeto

*   Inexperiência da equipe
*   Gerenciamento ineficiente do projeto
*   Requisitos instáveis
*   Falta de metodologia 
*   Tamanho do projeto

#### Métodos de estimativas empíricos

*   Estimativa Ad-hoc

*   Estimativa isolada. Projeto não está conectado a uma outra situação conhecida.

*   Estimativa gerencial

*   Gerente estima o prazo. Problema de prazo sub-dimensionado.

*   Métodos ágeis

*   planning poker, etc

*   De equipe

*   a própria equipe estima o trabalho
*   Pode ser feita utilizando uma técnica chamada Delphi: cada pessoa faz uma contagem e depois tenta-se convergir os valores

#### Reflexões sobre estimativas de software

*   Métricas são falíveis

*   Mesmo assim é melhor ter métricas do que planejar no escuro

*   Utilizar faixas de tolerância é uma recomendação
*   Não se consegue boas estimativas no início do projeto

*   Mesmo assim uma estimativa inicial deve ser feita

*   Uma base histórica é o que faz a diferença para uma boa estimativa

#### Outras métricas

*   COCOMO II

*   Bom para estimar custo. Difícil de ser usado.

*   Pontos de Caso de Uso

*   Derivada dos pontos de função, mas usa atores e casos de uso.

*   Pontos de histórias de usuário

*   aplicada em histórias de usuário dos métodos ágeis

*   COSMIC

*   Nova geração de métricas. Não estabelece limites para medição de uma função. Mede não somente a camada da aplicação mas a infraestrutura.
*   Deve ser aplicado quando há muita variação de escopo
*   Deve ser aplicado com muitos pontos de função
*   Propicia o aumento da previsibilidade e menor variabilidade na relação entre o tamanho, custo e esforço.
