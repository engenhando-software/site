title: "Banco de Dados Distribuidos"
date: 2015-02-22T16:12:00.001-03:00
updated: 2015-06-08T22:07:22.618-03:00
tags: 
- "disciplina4"
- "modulo1"
- "unidade2"
permalink: "banco-de-dados-distribuidos"
comments: true
---

Consiste num conjunto de bancos espalhados e um sistema distribuído para gerenciar esses bancos. Cada local pode realizar transações: locais, em que acessam dados de um único local e globais onde acessam dados em vários locais.  

### Condições mínimas para ser um banco de dados distribuído

*   Estar conectados em rede
*   Possuir uma inter-relação lógica dos bancos
*   Não é necessário que o software seja o mesmo em cada nó da rede

### Transparência

*   Usuário: usuário não precisa saber detalhes de implementação
*   Distribuição ou rede: usuário não precisa saber configuração de rede
*   Local: Usuário não sabe onde o banco se encontra
*   Nomes: nome dos dados. usuário chama um dado pelo nome que ele conhece.
*   Replicação e Fragmentação: usuário não precisa saber como o dado está.
*   Projeto: Projeto do banco de dados é transparente ao usuário
*   Execução: Como deve ser feita a requisição e o processamento no banco, usuário não precisa saber;

### Custo de instalação de um banco de dados distribuído

1.  Custo de instalação: tempo para ligar fisicamente um nó
2.  Custo de comunicação: custo em tempo e dinheiro para enviar uma mensagem entre os nós
3.  Confiabilidade: frequência com a qual uma ligação apresenta falhas
4.  Disponibilidade: o grau com que um dado pode ser acessado ainda que algumas apresentem falhas

### Prós e Contras à distribuição de dados

#### Vantagens

*   Autonomia local, mesmo que a rede esteja indisponível, o sistema se mantem localmente
*   Confiabilidade e Disponibilidade: forte ponte do BDD.
*   Aceleração do processo de consulta: pode-se subdividir uma consulta que são executadas em paralelo
*   Crescimento incremental: cresce de acordo com a necessidade

#### Desvantagens

*   Aumento da sobrecarga de processamento: sistema deve encontrar o dados no nó correto
*   Maior chance de erros
*   Custo de desenvolvimento do software

### Tipo de Sistemas de BDD

Características:

*   **(Hetero)Homogeneidade**: é a diferença de sistemas (ou SGBD) entre os bancos distribuídos. Um banco é homogêneo quando ele tem mesmo sistema em todos os nós.
*   **Autonomia**: quando cada local possui seu próprio banco de dados. O dados podem ser acessados em qualquer lugar, por isso, se um nó cair, o sistema continua funcionando obtendo o dado de outro nó.
*   **Distribuição**: é o quanto o banco é distribuído.

                          **Autonomia    Distribuição   Heterogeneidade****Centralizado**       total                 nenhuma          nenhuma**Puros**                   nenhuma          alta                   nenhuma**Federado**             media               alta                   alta **Multibancos**        alta                   alta                   alta  

### Dificuldades com bancos federados

*   Diferenças entre linguagens, restrições, interpretação quando um banco está muito distante, p.ex., Brasil x EUA.
*   Diferença entre nome de um dado, p.ex., mexerica, pocan, tangerina e bergamota. Os nomes referenciam ao mesmo produto, mas cada local tem um nome diferente.
*   Forma como realizar agregação de tabelas e resumos

### Replicação 

*   Síncrona: o dado é replicado na mesma hora (traz overhead)
*   Assíncrona: o dado é replicado na hora que o SGBD achar melhor

### Fragmentação

*   Horizontal: linhas de uma tabela
*   Vertical: colunas de uma tabela (exige o "id de tupla", maior sobrecarga)
*   Mista: SGBDs ainda não implementam 

### Estrutura de um BDD

GT - é o mesmo componente do SGDB centralizado  

Todo nó possui um Gerenciador de Transações (GT) que cooperam entre si para execução das transações. É responsável por manter o log, participa do controle de concorrência.O **coordenador de transações** coordena as transações locais e globais. É responsavel por  

*   iniciar uma transação; 
*   distribuir a transação nos nós apropriados;
*   coordernar a conclusão da transação.

### Robustez

Um SGBD é robusto quando consegue detectar falhas, reconfigurar o sistema para continuar o funcionamento e recuperar a situação original.

###   
Two-Phase Commit

Coordenador emite uma mensagem para o GT, dizendo que vai atualizar. O GT responde OK, o coordenador envia a mensagem para o GT com a forma para atualizar. Se o coordenador não responder um segundo OK ele aborta a transação.São duas fases, uma o coordenador pergunta se pode atualizar e a outra confirma se foi atualizado.

### Three-Phase Commit

Agora há um pré commit entre as duas fases do Two-Phase Commit.
