title: "Gerência de Configurações"
date: 2015-07-03T21:42:00.004-03:00
updated: 2015-09-06T17:11:18.275-03:00
tags: 
- "disciplina4"
- "modulo2"
- "unidade3"
permalink: "gerencia-de-configuracoes"
comments: true
---

A Gerência de Configuração tem por objetivo cuidar dos ativos de um projeto de software, tais como  

*   Programas;
*   Documentação Técnica;
*   Documentação Gerencial;
*   Informações sobre projetos e indicadores;
*   Etc.

No RUP, a disciplina que cuida dessa parte é a Gerência de Configuração e Mudança.

### Exemplos de ferramentas de GC

*   SVN
*   Tortoise
*   Subversion
*   MS Sharepoint
*   IBM Clearcase

### Conceitos de gerenciamento de mudanças

*   **SCM (Gerência de Configuração)** é uma atividade que abrange e é aplicada em todo processo de engenharia de um software. Como as mudanças podem ocorrer a qualquer tempo, as atividades de SCM são desenvolvidas para (1) identificar mudanças; (2) controlar mudanças; (3) garantir que a mudança esteja sendo adequadamente implementada; e (4) ressaltar a mudança a outras pessoas que possam ter interesse nela. Pressman
*   Uma **configuração** descreve um estado temporal que um elemento se encontra. Deve conter todos elementos significativos daquele sistema, tais como, estado do hardware, do software, documentação técnica relevante, bibliotecas, etc.
*   **Controle de versão** é o controle das revisões, mudanças na evolução de um item de produto. Objetivos:

*   Automatizar o rastreamento de arquivos
*   Prevenir conflitos de desenvolvedores
*   Recuperar versões previas
*   Permitir o desenvolvimento paralelo
*   Auditar o desenvolvimento
*   Reduzir o espaço de armazenamento
*   Estabelecer relacionamento entre arquivos, versões e distribuições

*   **Gerencia de configuração** controla as revisões, mudanças e dependências de um item de produto. Portanto, gerencia de configuração é mais amplo que controle de versão.
*   **Item de configuração** são itens que devem ser mantidos sob o controle da gerencia de configuração. São itens individuais. Ex. versão da espec. de requisitos, código fonte, cronograma de projeto, planilha de verificação.
*   **Baseline** é uma versão formalmente aprovada de um item de configuração, independente de mídia, formalmente definida e fixada em um determinado momento durante o ciclo de vida do item de configuração. Ou seja, é o estado inicial de configuração de um projeto. Os principais tipos, são:

*   Funcional: proposta do desenvolvimento de sistemas
*   Alocação: especificação de requisitos
*   Projeto: especificação de implementação e revisão critica
*   Produto: doc. de implementação, plano de teste e aceitação
*   Operacional: doc. comprova a aceitação do usuário

*   **Repositório** é um local sobre controle de acesso, onde são armazenados os itens de configuração de software.
*   **Build** representa uma versão ainda incompleta do sistema mas com certa estabilidade. Inclui outros docs, além do fonte.
*   **Branches e Trunks**, são ramificações laterais de versões que se originam de uma revisão da linha principal de desenvolvimento.
*   **Versão alfa**, é uma versão produzida após um ciclo de desenvolvimento e utilizada em testes controlados
*   **Versão de homologação ou beta**, é liberada aos clientes para testes
*   **Versão oficial**, liberada comercialmente para clientes
*   **Versões emergenciais** visa resolver bugs
*   **Checkout** quando se obtém uma cópia da versão do arquivo para modificação e simultaneamente se impede o acesso a outros usuários. Checkin quando se cria uma nova versão do arquivo e se libera o acesso a essa nova versão.

### Funções da Gerencia de Configuração

1.  Identificação de configuração

*   Tem como objetivo a seleção dos itens de configuração desejados;
*   Definição de um esquema de codificação
*   Descrição dos itens

3.  Controle de configuração

*   Permite o acompanhamento da evolução dos itens de configuração. Estabelece as atividades para que os itens possam evoluir de forma controlada:
*   (1) solicitação de modificação, iniciando o ciclo de controle para uma manutenção
*   (2) classificação da modificação
*   (3) análise de impacto
*   (4) avaliação da modificação pelo comitê de controle de configuração
*   (5) implementação da modificação
*   (6) verificação da modificação com relação à proposta de implementação levantada
*   (7) atualização da baseline 

5.  Contabilização de configuração

*   Possui duas responsabilidades:
*   (1) Armazenar informações geradas pelas demais funções
*   (2) Permitir que as informações possam ser acessadas

7.  Avaliação e revisão da configuração

1.  Ocorre quando a baseline (gerada no controle de configuração) é selecionada para ser liberada para o cliente. Suas atividades são:
2.  (1) Auditoria funcional da baseline
3.  (2) Auditoria física de baseline

9.  Gerenciamento de liberação e entrega

1.  Construção: produzindo novos itens de configuração
2.  Liberação: identificado versões particulares de cada item de configuração
3.  Entrega: implantando produto no ambiente final de produção

### Papeis, Artefatos e Atividades de GC

*   Gerente de configuração: papel de controlar as configurações de software
*   Auditor de configuração: responsável pela auditoria dos projetos
*   Equipe de projeto: usuários da gerencia de configuração de software
*   Bibliotecário: responsável pelo acesso a biblioteca de configurações (repo)
*   Comitê Controle de Mudança: responsável pelas decisões de modificação

### Gerência de Configuração MPS-BR

Pertence ao <span style="background-color: yellow;">Nível F</span> junto com as atividades de 

*   Aquisição
*   Garantia da qualidade
*   Medição
*   Gerência de portfólio de projetos

GCO é composta por 7 REPs (Resultados Esperados no Processo), apresentados a seguir:

*   GCO1 - Um Sistema de Gerência de Configuração é estabelecido e mantido;
*   GCO2 - Os itens de configuração são identificados com base em critérios estabelecidos;
*   GCO3 - Os itens de configuração sujeitos a um controle formal são colocados sob baseline
*   GCO4 - A situação dos itens de configuração e das baselines é registrada ao longo do tempo e disponibilizada;
*   GCO5 - Modificação em itens de configuração são controladas;
*   GCO6 - O armazenamento, o manuseio e a liberação de itens de configuração e baselines são controlados;
*   GCO7 - Auditorias de configuração são realizadas objetivamente para assegurar que as baselines e os itens de configuração estejam íntegros, completos e consistentes.

O objetivo da GCO é <span style="background-color: yellow;">estabelecer e manter a integridade de todos os produtos de trabalho</span> de um projeto e disponibiliza-los para equipe.
