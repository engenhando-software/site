title: "Projeto Arquitetural"
date: 2015-05-17T11:49:00.000-03:00
updated: 2015-09-05T16:31:06.423-03:00
tags: 
- "disciplina2"
- "modulo2"
- "unidade3"
permalink: "projeto-arquitetural"
comments: true
---

## Fundamentos da Análise Arquitetural

Trata de modelos que ajuda o implementador a construir o software.  

### Questões Principais

*   Como decompor um sistema em diversos pacotes e subsistemas?

*   Quais classes devem estar em cada subsistema de forma a permitir mais reutilização de subsistemas?
*   Quais dependências entre os subsistemas?
*   Quais os conectores devem ser usados entre os subsistemas?

*   Como distribuir cada um dos subsistemas em diferentes nós de processamento?

*   Apenas um subsistema em cada maquina ou mais de um?
*   Qual o impacto no resto do sistema se agruparmos ou separarmos subsistemas em diferentes nós?

###  Propriedades do sistema

*   Escala: número de usuários 
*   Capacidade: de atender ao um certo número de requisições
*   Degradação: como o sistema se comporta (degrada) se a capacidade for ultrapassada
*   Desempenho
*   Portabilidade

### Projeto arquitetural identifica:

*   Componentes: definem onde ocorre o processamento;
*   Conectores: mediam as interações entre os componentes;
*   Propriedades: informações para a construção e análise;

### Modelo "4+1" visões arquiteturais

[![](http://4.bp.blogspot.com/-AzX4hvxeaS8/VVeHiZ4fMSI/AAAAAAAAC7Q/6qvlAFL2EFs/s400/slide_3.jpg)](http://4.bp.blogspot.com/-AzX4hvxeaS8/VVeHiZ4fMSI/AAAAAAAAC7Q/6qvlAFL2EFs/s1600/slide_3.jpg)

*   Visão de projeto ou lógica: estamos interessados em definir a funcionalidade do sistema, vocabulário dos objetos de negócio do sistema
*   Visão de implementação ou componentes: definir o gerenciamento da configuração, quais os elementos que vão fazer parte da configuração do sistema. Aqui definimos como fazer o build do sistema.
*   Visão de processo: interessados na visão de execução do sistema, nessa etapa que nos preocupamos com as propriedades do sistema (acima). 
*   Visão de implantação: mostra como os componentes de software estão mapeados pelos componentes de hardware. (Topologia, distribuição, fornecimento, instalação, etc)
*   Visão de caso de uso: diagrama de casos de uso.

> A visões são como as diferentes visões de uma casa, como a planta baixa, projeto elétrico, projeto hidráulico, maquete 3D, etc.

### Pontos de Variação e Evolução 

*   Pontos de Variação: variações previstas nos requisitos do sistema.
*   Ponto de evolução: pontos especulativos de variação que podem surgir no futuro mas que não estão presentes nos requisitos existentes.

**Passos para fazer análise arquitetural:**

*   Identificar e analisar os requisitos não-funcionais e funcionais
*   Analisar alternativas e criar soluções que resolvam o impacto, documentando as decisões arquiteturais

**Fatores arquiteturais**

*   Segurança

*   Como o controle de segurança afeta o projeto do sistema para evitar uso indevido do sistema?

*   Confiabilidade, tolerância a falhas

*   Como os requisitos de confiabilidade e tolerância a falhas afetam o projeto?

*   Custo

*   Custo de software de terceiros adquiridos vai afetar os lucros, etc.

*   Adaptabilidade, configurabilidade

*   Como afetam o projeto?

*   Desempenho, capacidade e degradação

*   Como afetam o projeto?

*   Usabilidade

*   Como impacta no projeto?

*   Restrições de projeto

*   Como as interfaces externas com outros sistemas, o ambiente de desenvolvimento e execução impactarão na solução?

*   Restrições de Processo

*   Como a documentação exigida, normas e processos a serem seguidos no desenvolvimento vão impactar a arquitetura?

## Padrões Arquiteturais

São formas conhecidas para se estruturar um sistema. Se diferem um dos outros nos componentes, nas formas de conexão e formas de se conectar.**Categorias de padrões arquiteturais**

*   Sistemas de fluxo de dados;

*   Disponibilidade dos dados controla a computação;
*   Estrutura baseia-se na transferência ordenada de dados entre componentes;
*   Não há outra forma de interação entre componentes;
*   Variações: Batch sequencial, pipe-e-filtro e padrão de camadas;
*   Exemplo: comunicação entre camadas de redes (ISO/OSI)

*   Sistemas de chamada-e-retorno;
*   Sistema em rede;

*   Cliente-servidor: 

*   Em geral, clientes iniciam as computações e interagem com usuários. Servidores: executam as computações e provêm recursos.

*   P2P

*   Componentes executam em máquinas distintas;
*   Cada componente age como ambos, cliente e servidor.
*   Em geral, existe um servidor centralizado onde os componentes se registram.
*   É um padrão resiliente. Tolera a remoção de componentes.

*   Sistemas interativos;
*   Repositórios;
*   Sistemas orientados a serviços;

*   Componentes são serviços de organizações possivelmente diferentes (provedores).
*   Conectores são XML
*   Aplicações que requisitam os serviços, são os consumidores
*   Existe um diretório de serviços (banco de dados) onde eles podem ser descobertos
*   Requisitante pode ser uma aplicação, web service, mobile, etc.

*   Computação nas nuvens

*   Funcionalidade é toda através de serviços
*   Está fora da empresa que necessita do serviço
*   As maquinas são virtualizadas. Configuradas de acordo com a necessidade, como o S.O.
*   Os recursos são escaláveis
*   Gerenciamento
*   Serviços são providos no modelo de pilha

*   IaaS: Infra Ex: EC2 (Amazon)
*   PaaS: Plataforma Ex: Google AppEngine, MS Azure
*   SaaS: Software (Aplicação) Ex: SalesForce

[![](http://1.bp.blogspot.com/--OZ4gvN-j_s/VVijNYNrVOI/AAAAAAAAC7k/WMD_ZXa9bPE/s320/Divisao%2Bcloud.jpg)](http://1.bp.blogspot.com/--OZ4gvN-j_s/VVijNYNrVOI/AAAAAAAAC7k/WMD_ZXa9bPE/s1600/Divisao%2Bcloud.jpg)  

## Arquitetura na UML

Voltar no modelo 4+1

*   Visão de casos de uso

*   É um resumo dos casos de uso mais significativos
*   Ilustra a cobertura arquitetural mais significativa
*   O caso de uso "Processar Venda" exercita vários elementos arquiteturais, por isso, é interessante detalhar. Podemos incluir realizações, contratos de operação, diagramas de interação.

*   Visão lógica ou de projeto

*   Mostra a organização conceitual do software, em termos de camadas, subsistemas, pacotes, frameworks, classes importantes.
*   É uma visão para o modelo de projeto do RUP

*   Visão de implementação ou de componentes

*   Inclui os componentes utilizados para montar e entregar o sistema físico
*   Um componente de software é uma unidade indivisível de um sistema. Ex: Banco de dados, navegador web.

*   Podem ser substituídos por outros componentes que fazem a mesma coisa
*   Caixa preta com interface bem definida
*   Fornece ou requisita serviços a outros componentes

*   Visão de implantação

*   Representa a topologia física do sistema e componentes que são executados nessa topologia. Mostra um mapeamento entre elementos de hardware e software.
*   Elementos do diagrama são os nós de processamento e conexões.

*   Nós: processadores, sensores, etc. (executam software)
*   Conexões: meio físicos de comunicação (cabos), ou protocolos (tcp, etc)

### Arquitetura na UML

Como representar arquitetura na UML, utiliza os conceitos de:

*   Pacotes

*   É um mecanismo para agrupar vários artefatos de um modelo
*   Podem conter outros pacotes
*   Podem existir relacionamentos entre pacotes

*   Interfaces 

*   É um conjunto de especificações de serviço
*   Não contém estrutura interna (diferente de uma classe abstrata)
*   Quando uma classe implementa as operações de uma interface, a classe realiza essa interface

*   Subsistemas
