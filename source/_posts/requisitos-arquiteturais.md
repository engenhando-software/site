title: "Requisitos Arquiteturais"
date: 2015-09-19T13:07:00.002-03:00
updated: 2015-12-05T15:19:21.164-02:00
tags: 
- "disciplina2"
- "modulo3"
- "unidade2"
permalink: "requisitos-arquiteturais"
comments: true
---

## Requisitos arquiteturais

Não são requisitos não-funcionais. São requisitos que de alguma forma afetam a arquitetura.Dado um requisito

> O sistema deve ser **rápido** e capaz de processar **grandes quantidades** de requisições simultâneas

"Rápido" e "grandes quantidades" são atributos de qualidade chamados performance e escalabilidade, respectivamente. Ainda nesse requisito, fala de todo o sistema, ou seja, é muito genérico. O papel do arquiteto é transformar um requisito como esse em um requisito específico e mensurável. Um exemplo de um requisito esperto seria:  

> A **tela de cadastro** de usuários deve possuir um tempo de resposta menor que **8 segundos** e suportar **20 usuários** simultaneamente em horários de pico (15:00 às 19:00).

## Modelo FURPS+

O modelo permite capturar e qualificar requisitos com completude ao longo do projeto.  

Devemos capturar requisitos ao longo de cinco dimensões:  

*   Functionality - Funcionalidade
*   Usability - Usabilidade
*   Reliability - Confiabilidade
*   Performance - Desempenho
*   Supportability - Suportabilidade

Dimensão adicional que lida com restrições técnicas:  

*   Restrições ao desenho
*   Restrições à implementação
*   Restrições de interface
*   Restrições físicas

### Funcionais

#### Funcionalidade

*   Lida com aspectos funcionais
*   Requisitos funcionais que o sistema deve atender
*   Geralmente relacionados ao domínio do problema
*   Ex. pequisa de palavras chave do google (muito complexo)
*   Segurança, ajuda on-line, log de auditoria, controle de licenças, envio e recebimento de e-mails, i18n, recursos de impressão e relatórios, recursos de work

### Não funcionais: URPS

#### Usabilidade

*   Qualidade da interação entre o sistema e o usuário final. Ex: Velocidade que o usuário entre e recupere informações, facilidade de aprendizado para usuários leigos. 

#### Reliable (Confiabilidade)

*   É a disponibildiade do sistema. Qual o tempo que o sistema está disponivel? 
*   Ex: um produto com disponibilidade de 99% do tempo ao longo de 24 horas. 
*   Outro exemplo é a recuperação de falhas. Dado uma falha, qual o tempo que o sistema demora para se recuperar.

#### Performance (Desempenho)

*   Está relacionado a dois itens: Vazão e Tempo de resposta
*   Vazão: associada ao processamento em lote. Ex. processar folha de pagamento
*   Tempo de resposta: tempo que o sistema demora pra fazer uma requisição.

#### Supportability - Suportabilidade

*   Está relacionado aos aspectos internos do sistema, onde somente a equipe de TI consegue enxergar e não o usuário final.
*   Ex: Manutenabilidade, sistema operacional

#### Restrições

Elementos que precedem um determinado produto ou escolha a ser feita. Ex: a empresa já usa um banco Oracle, ou a tela de dispositivo é de 3,5'.  

*   Restrição ao desenho: especifica e restringe as opções de arquitetura do sistema
*   Restrição à implementação: especifica e restringe os aspectos de implementação de código
*   Restrição de interface: É uma restrição de comunição. Ex. o sistema deve interoperar através de Webservice
*   Restrição física: restrições de algum tipo de hardware
