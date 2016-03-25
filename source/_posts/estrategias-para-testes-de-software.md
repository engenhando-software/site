title: "Estratégias para testes de software"
date: 2015-08-19T21:59:00.000-03:00
updated: 2015-12-05T11:35:49.904-02:00
tags: 
- "disciplina1"
- "modulo3"
- "unidade3"
permalink: "estrategias-para-testes-de-software"
comments: true
---

## Estratégias para teste de software URL

*   Testes de módulos atômicos

*   Usa testes de caixa branca

*   Testes de integração
*   Testes de validação

*   Caixa preta

*   Testes de sistema

*   Desempenho, segurança

*   Testes de aceitação

*   No ambiente do usuário

### Testes de módulos atômicos

*   Testar condições limite
*   Todos os caminhos são testados (método caminho básico)
*   Usa-se Drives que são chamadas aos módulos (que simulam um modulo ainda não testado)

### Testes de integração

Consiste em se integrar os módulos do sistema. Possui duas abordagens:

*   Bottom-up

*   Parte para os módulos no nível mais baixo. Os módulos são agrupados em clusters para que fique mais fácil de testar e cria-se drivers que vão simular uma parte superior na estrutura da hierarquia dos módulos que ainda não foi testada. 
*   Vantagem: São mais simples que o top-down.

*   Top-down

*   Parte para os módulos de nível mais alto. Há duas formas de percorrer os módulos para testes: Profundidade - testa-se verticalmente até chegar numa folha - e Largura no qual se testa horizontalmente cada nível. 
*   Stubs = mock

### Testes de validação

*   Uma sequencia de testes de caixa-preta que demonstram a funcionalidade dos requisitos.
*   Os casos de teste devem ser montados seguindo a especificação de requisitos
*   Depois de realizar cada caso de teste, vão existir uma das opções

1.  Teste é aceito 
2.  Uma lista de deficiências é criada

### Testes de sistema

Tem como objetivo colocar o sistema à prova. Tipo mais comuns:

*   Testes de recuperação: forçar o sistema a falhar e ver a recuperação do sistema
*   Testes de segurança: verificar os mecanismos de segurança do sistema. Senhas, proteção de acesso a funções. recomendável um especialista.
*   Teste de stress: consiste em testar o programa em situações limite
*   Testes de desempenho: realizado para testar os requisitos de desempenho descritos na especificação. Deve ocorrer ao longo de todos os passos do processo de testes. Confundido com teste de stress.

### Testes de aceitação

Visam especificamente capacitar clientes a validar seus requisitos. Realizado exclusivamente pelo usuário final. 

*   Alfa teste: realizado nas instalações do desenvolvedor
*   Beta teste: realizado nas instalações do cliente

## Revisões formais

As revisões capturam erros durante as etapas de desenvolvimento e evita que esses erros sejam descobertos no fim do desenvolvimento.

#### Tipos de revisões:

*   Revisão de especificação é uma revisão em que os requisitos e especificações do usuário são revisados
*   Revisão de interface do usuário: preocupa-se com os formatos de entrada e saída, layout de tela, relatório, posição dos componentes na tela, etc. Do campo IHC.
*   Revisão de projeto é revisão dada nas decisões de implementação, arquitetura de software, técnicas empregadas, etc.
*   Revisão de código: verifica o código fonte
*   Revisão de teste: conduzidas para que os dados de teste sejam adequados ao sistema, não pra examinar a saída do teste.

#### Papeis:

*   Apresentador: a tarefa é introduzir o produto, apresenta o produto numa reunião.
*   Coordenador: responsável para que as atividades sejam organizadas e atua também como moderador.
*   Secretário copista: tomar notas durante da revisão
*   Oráculo da manutenção: rever o produto sobre manutenções futuras
*   Portador de padrões: especialista em engenharia de software que verifica se normas e padrões estão sendo seguidos
*   Representante do usuário: verifica se os requisitos estão sendo atendidos
*   Especialista na área do sistema: verifica se o sistema está correto na área da especialidade. Ex.: folha de pagamento.

#### Responsabilidades do autor

*   Anunciar sua intenção de fazer uma revisão
*   Escolher participantes e coordenador
*   Fornecer material apropriado para a revisão
*   Escolher um produto que possa ser revisado em no máximo 60min.

#### Responsabilidades do coordenador

*   Assegurar que a revisão aconteça;
*   que os participantes atendam a revisão
*   Distribuir o material para a revisão

#### Responsabilidades dos outros membros

*   Ler documentação fornecida antes da reunião (1 hora)

#### Ao final da revisão:

*   Coordenador notifica a gerencia
*   É distribuída uma cópia da ata aos participantes
*   Produtor vai realizar as ações descritas na ata
