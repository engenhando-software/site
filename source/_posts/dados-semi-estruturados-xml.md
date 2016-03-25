title: "Dados Semi-Estruturados XML"
date: 2015-03-08T12:25:00.000-03:00
updated: 2015-06-05T22:25:29.347-03:00
tags: 
- "disciplina4"
- "modulo1"
- "unidade1"
permalink: "dados-semi-estruturados-xml"
comments: true
---

O que são:

*   Dados Estruturados: são os dados contidos nos bancos de dados, com formato definido.
*   Dados Semiestruturados: são dados que permitem adicionar atributos mesmo depois de criados.
*   A diferença entre os dois então, é a forma de criação do schema.

### Linguagens de Marcação

*   **HTML** foi a primeira. Trabalha com marcadores definidos. Cuida da forma como o dado é apresentado. A visualização é sempre fixada (ex. o dado é sempre em itálico).  
*   **XML** nasceu para tratar do do conteúdo dos dados, trouxe flexibilidade, e não existe nenhuma preocupação com a  apresentação dos dados. Possui uma estrutura hierárquica. 

#### Utilização da XML

*   Busca de dados na web
*   Troca de dados
*   Catálogos
*   Automação de grandes redes (bancos, suprimentos, etc.)

#### Linguagens para manipular XML

*   Xpath: trabalha através de grafos, para saber o caminho percorrido
*   Xquery: voltada para recuperar o dados
*   XSL: definir o estilo que o dados serão exibidos

### Conceitos de XML

*   Documento bem formado: ordem de abertura e fechamento das tags
*   Documento válido: de acordo com o esquema definido

### DTD (Document Type Description) 

Contém as regras para elaboração do XML. Define que um XML pode conter, a ordem, obrigatoriedade, cardinalidade (número de vezes que cada valor ocorre) e unicidade (se possui valor único ou não). Pode estar dentro ou fora do arquivo XML.

#### Declarações contidas em uma DTD

*   ELEMENT: especifica um elemento do XML
*   ATTLIST: declara uma lista de atributos associados a um elemento e o valores possiveis
*   ENTITY: usado para declarar uma espécie de alias dentro do doc.
*   NOTATION: usado para passar dados sobre impressora, ou a forma de impressão do doc.

### Descrição de cada declaração

Tag ELEMENT  

<!ELEMENT S Nome S EspecificacaoConteudo S ?>  

*   Nome - nome do elemento
*   EspecificaçãoConteudo pode ser:

*   EMPTY - não possui nenhum dado no elemento
*   ANY - pode ser vazio ou não
*   mixed - pode ter alguma informação dentro dele ou alguns filhos
*   children - subdivide-se em outros elementos

*   ? (Cardinalidade) pode ser

*   ? -> No máximo uma ocorrência
*   * -> Nenhuma ou diversas ocorrências
*   + -> No mínimo uma ocorrência

Simbolo "|" -> o elemento pode se dividir em outros elementos e eles são alternativos  
Tag ATTLIST  
<!ATTLIST S Nome S EspecificacaoAtributo S ?>  

*   Nome - nome do atributo
*   EspecificacaoAtributo é composto por:

*   NomeAtributo S TipoAtributo S ValorPadrão S ValorDefault
*   Onde:
*   NomeAtributo - nome do atributo
*   TipoAtributo são os tipos:

*   CDATA: dados com formato de caracteres (não pode conter tag)
*   ID: identificador do elemento (possui valor único)
*   IDREF: é a referencia ao ID de um atributo
*   IDREFS: mais de um ID
*   NMTOKEN: palavra ou conjunto de palavras sem espaço 
*   NMTOKENS: lista separadas por espaço 
*   ENUMERADO: lista enumerada

*   ValorPadrão - sempre será esse valor, não muda nunca
*   ValorDefault - se nao definir um valor pro atributo, ele assume esse valor padrão

*   ? Cardinalidade - mesma do elemento
