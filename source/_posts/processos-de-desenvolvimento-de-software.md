title: "Processos de desenvolvimento de software"
date: 2014-09-24T22:18:00.000-03:00
updated: 2015-04-04T15:54:25.599-03:00
tags: 
- "disciplina1"
- "modulo1"
- "unidade2"
permalink: "processos-de-desenvolvimento-de-software"
comments: true
---

### Citações

> Software de qualidade é aquele que atende seus requisitos

> Processo de software é uma metodologia para as atividades, ações e tarefas necessárias para desenvolver um software de alta qualidade.

> Uma ideia proposta por uma série de renomados engenheiros de software: um processo de software deve priorizar flexibilidade, extensibilidade e velocidade de desenvolvimento, acima da alta qualidade.

> Quando restrições cruzam múltiplas funções, recursos e informações do sistema, elas são, frequentemente, denominadas restrições cruzadas. (Aspecto) 

### Atividades Metodológicas

São atividades genéricas que podem ser encontradas em qualquer processo de engenharia de software, ela define 5 passos essenciais:  

*   Comunicação
*   Planejamento
*   Modelagem
*   Construção
*   Entrega

### Atividades de Apoio (Umbrella activities)

Essas atividades complementam e auxiliam as atividades metodologicas, são elas:

*   Controle e acompanhamento do projeto
*   Administração de riscos
*   Garantia de qualidade
*   Revisões técnicas
*   Medição
*   Gerenciamento de configuração de software
*   Gerenciamento da reusabilidade
*   Preparo e produção de artefatos

### Fluxo de Processo

Todo o processo de engenharia de software segue um dos quatro tipos de fluxo de processo:  

*   Linear
*   Iterativo
*   Evolucionário
*   Paralelo

### Padrões de Processo

Nome do Padrão  
Forças  
Tipo (Padrão de estágio, tarefas ou fases)  
Contexto inicial  
Problema  
Solução  
Contexto Resultante  
Padrões relativos  
Usos conhecidos e exemplos  

#### Avaliação e aperfeiçoamento dos processos de software

*   SCAMPI (CMMI)
*   CBA IPI (CMM)
*   SPICE (ISO/IEC15504)
*   ISO 9001:2000

### Modelos de Software

#### Modelo de Processo Prescritivo

A engenharia de software e o seu "produto" beiram o caos, ao mesmo tempo que está tudo organizado, está muito próximo também de surpresas. O modelo de processo prescritivo tenta trazer ordem ao caos através de um conjunto de elementos de processo como, atividades metodologicas, ações de engenharia, tarefas, produtos de trabalho, garantia de qualidade, etc.Todos os modelos de processo de software (listados abaixo) podem acomodar as atividades metodologicas genéricas (comunição, planejamento, modelagem, construção e entrega).  
Os modelos de processo prescritvos são conhecidos como modelos tradicionais.  

#### 

*   Modelo em cascata

Também conhecido como ciclo de vida clássico e waterfall model. Existe uma variação desse modelo chamado Modelo V, em que a segunda parte existem testes que validam o software e se necessário pode-se corrigir antes de entregar o produto.  

*   Adia identificação de riscos
*   Atrasa os testes do sistema
*   Difícil entrega parcial do produto
*   Difícil lidar com mudança de requisitos

#### 

*   Incremental

<span style="font-weight: normal;">O modelo incremental aplica sequencias lineares, de forma escalonada, a medida que o tempo vai avançando. Cada sequência linear gera "incrementais" (entregáveis/aprovados/liberados) do software. Exemplo do editor de textos, a cada incremento, novas funcionalidades são adicionadas.</span>  
<span style="font-weight: normal;">  
</span>

#### 

*   Evolucionário (espiral e prototipação)

*   Prototipação (Problemas conhecidos)

*   <span style="font-weight: normal;">O cliente enxerga o prototipo como o software já pronto, e exige que com algumas modificações ele se torne operacional, constantemente a gerência de desenvolvimento aceita.</span>
*   <span style="font-weight: normal;">Na pressa de apresentar um protótipo, o engenheiro de software opta por ferramentas como liguagem de programação, sistema operacional que lhe são mais intimas simplesmente. Após um tempo, pode se acomodar com tais escolhas e o projeto acaba adotando definitivamente essas tecnologias, que podem não ser as ideais. </span>

*   Espiral

*   <span style="font-weight: normal;">Parecido com o incremental, o software evolui a cada volta na espiral.</span>

*   **Concorrente** 

Define uma rede de processos que são ligados e possuem estados como concluido, aguardando modificações, em exame, inativo, etc.  

#### Modelo de Processo Especializado

*   **Baseado em Componentes**

*   Esse modelo desenvolve aplicações a partir de componentes de software pré-empacotados.
*   As atividades de modelagem e construção desse modelo começam com a identificação de possíveis candidatos a componentes.

*   **Métodos formais**

*   Através de análise matemática são facilmente descobertos problemas no software como ambiguidade, incompletude e inconsistência
*   Desvantagens: consome muito tempo e dinheiro, poucos desenvolvedores capacitados, dificil comunicação com o cliente.

#### PSP (Personal Software Process)

O PSP enfatiza a medição pessoal do todo o processo desde o planejamento até a entrega do software. Com esses dados de medição coletados, o engenheiro de software pode trabalhar em melhorar as partes falhas do processo executados por ele mesmo. O PSP não foi largamente adotado pelo setor, os motivos têm mais a ver com a natureza humana e com a inércia organizacional do que propriamente com o processo desenvolvido por Watts Humphrey.

*   Planejamento
*   Projeto de alto nível
*   Revisão de projeto de alto nível
*   Desenvolvimento
*   Autópsia

#### TSP (Team Software Process)

Os principais objetivos do TSP são:

*   Equipes auto-dirigidas
*   Mostrar gerentes como treinar e manter equipes
*   Acelerar o aperfeiçoamento dos processos de software
*   Fornecer orientações para melhorias a organizações
*   Preparar universitário para trabalhar em equipe a nivel industrial

As atividades metodológicas do TSP são:

*   Lançamento do projeto
*   Projeto de alto nivel
*   Implementação
*   Integração e testes
*   Autópsia

Assim como o PSP, essa metodologia induz a equipe a se auto-avaliar, atraves de medições do processo e do produto. -----------------------------

#### UP (Unified Process)

É uma metodologia de processo. Foi criado pelo mesmos autores da UML. Possui três características chave:

*   Dirigido por casos de uso
*   Centrado na arquitetura
*   Iterativo e incremental

#### Fases do RUP

*   Concepção (comunicação e planejamento)
*   Elaboração (comunicação e modelagem)
*   Construção (construção)
*   Transição (última parte da construção e primeira parte da atividade de entrega)
