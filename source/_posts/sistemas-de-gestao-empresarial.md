title: "Sistemas de Gestão Empresarial"
date: 2015-03-05T23:30:00.001-03:00
updated: 2015-06-06T22:01:17.254-03:00
tags: 
- "disciplina4"
- "modulo1"
- "unidade4"
permalink: "sistemas-de-gestao-empresarial"
comments: true
---

## Sistemas de Gestão Empresarial

Existem dois grandes tipos de aplicações:  

*   **aplicações do negócio:** suportam o negócio e a parte administrativa do mesmo;
*   **aplicações sobre o negócio:** analisam e ajudam a interpretar o que ocorreu e a decidir estratégias futuras.

### Data Warehouse

É um armazém de dados, orientada por assuntos, integrada, variante do tempo e não volátil.

*   **Assuntos:** vendas de produtos, RH, aplicações financeiras
*   **Integrado:** se integra no banco da empresa
*   **Variante do tempo:** a chave principal da analise é o tempo
*   **Não volátil:** não se muda o dado

### Classificação

*   **Ambiente físico:** centralizado ou descentralizado
*   **Distribuição por função:** cada assunto fica em um data warehouse e todos se combinam para um objeto comum
*   **Camadas:** os dados resumidos ficam em um servidor, os com detalhamentos intermediário em outro e outro com dados atômicos  

### Data Warehouse e Metadados

Os metadados são divididos em três camadas:

1.  Operacionais (nível de aplicação): definem a estrutura dos dados mantidos pelos bancos operacionais.
2.  Centrais do data warehouse: metadados do próprio data warehouse 
3.  Nível do usuário: mapeiam os metadados do data warehouse para conceitos que sejam familiares ao usuário 

Classificação segundo classes de componentes:  

*   mapeamento: descrevem as transformação dos dados operacionais até chegarem ao data warehouse
*   histórico: quais mudanças existentes nos dados 
*   miscelânea: sinônimos

### Linguagens em banco de dados

*   OLTP: é o que estamos acostumados (SQL) 
*   OLAP: é usada em data warehouse (não faz a manutenção dos dados)

OLAP x SQL

*   SQL convencional tem pouco suporte a consultas temporais
*   SQL não dá suporte para otimizar um grupo de consultas, somente uma única

### Modelagem de Data Warehouse

*   Dimensão: é uma entidade, através dela que conseguimos apurar. Exemplos: marca, modelo de um veículo. São diferentes perspectivas envolvidas em cada projeto em uma organização
*   Fatos: são medições, numéricas. 

*   Aditivos: medições em uma tabela que podem ser adicionados ao longo de todas as dimensões, ex: quant. produtos vendidos
*   Semi-aditivo: fato numérico, que pode ser adicionado ao longo de algumas dimensões. Ex. estoque (nem sempre pode ser armazenados para todas as dimensões
*   Não aditivo: são fatos que não podem ser adicionados em qualquer dimensão, ex. textuais

*   Granularidade: nível de detalhes que são armazenados
*   Grão: significado de uma linha na tabela de fatos. Ex a quantidade de veículos armazenados podem ser computados por dia, mês, ano. Se for armazenado por grão "mês", não é possível recuperar por semana ou dia

### Modelos de data warehouse

*   Estrela (favorece aglutinação)

*   A tabela de fatos fica no centro do modelo e as dimensões ao redor.

*   Floco de Neve

*   Uma dimensão depende de outra. Para se apurar os fatos, deve-se ligar a uma dimensão e depois em outra. Ex. Produto > Categoria > Marca. 

Modelagem de um data warehouse

*   Orientado no negócio e necessidade do usuário
*   dados já foram produzidos
*   a normalização nem sempre se aplica
*   Diretrizes

*   o modelo dimensional deve se parecer com o corporativo
*   combinar a necessidade de informação com os dados disponíveis 

### 9 passos de decisão (KIMBALL)

1.  conhecer os processos (identidade dos fatos)
2.  decidir a granularidade de cada tabela de fatos
3.  decidir as dimensões da tabela de fatos
4.  quais fatos armazenar, que tipo de aglutinação
5.  definir os atributos de cada dimensão
6.  como rastrear dimensões de modificações mais lentas
7.  decisões de armazenamento físico
8.  amplitude de tempo histórico (terá uma visão de quanto anos atras?)
9.  definir os intervalos de extração dos dados

### Mineração de Dados

Regras

*   Associação: associar dados a outros dados
*   Sequenciais: informação é requerida depois que algum outro dado foi requerido (passagem aérea, hotel)
*   Classificação: indicadores estatísticos (frequência de visitas a loja, incidência de erros de empregados)

### Objetivos do Processo de Mineração

*   Previsão: prever fatos que já ocorreram no passado e podem ocorrer denovo
*   Identificação: identificar para minimizar ou maximizar a ocorrência
*   Classificação: classificar o que ocorre na organização
*   Otimização: otimizar os fatos ocorridos no passado
