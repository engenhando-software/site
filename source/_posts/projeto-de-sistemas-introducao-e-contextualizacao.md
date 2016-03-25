title: "Projeto de Sistemas: Introdução e Contextualização"
date: 2015-05-03T23:56:00.000-03:00
updated: 2015-09-05T12:00:44.250-03:00
tags: 
- "disciplina2"
- "modulo2"
- "unidade1"
permalink: "projeto-de-sistemas-introducao-e-contextualizacao"
comments: true
---

Objetivos do projeto de software:  

*   Definir um modelo implementável que atenda aos requisitos
*   Garantir que todos os requisitos sejam satisfeitos

#### Atividades de projeto

*   Projeto da arquitetura do sistema

*   Decomposição em componentes
*   Definição da interface entre eles

*   Projeto das interfaces do sistema

*   com usuário
*   com outros sistemas

*   Projeto detalhado comportamental

*   Projeto dos objetos e suas interações
*   Projeto da persistência de dados

*   Documentação do projeto

#### Avaliação do projeto (considerar a qualidade do projeto)

*   Determina se o projeto satisfaz os requisitos do sistema

*   Importante verificar se todos os requisitos foram considerados
*   Como o projeto atende/satisfaz um requisito

*   Determina se o projeto pode ser entendido pelos implementadores e testadores do sistema

#### Diagramas que contemplam a etapa de projeto 

*   Casos de uso

*   Diagrama
*   Especificação do caso de uso

*   Diagrama de Classes
*   Diagrama de Sequencia

*   Superficial (ainda na analise)
*   Detalhado

*   Diagrama de Componentes (projeto arquitetural)
*   Diagrama de Implantação

### Princípios de Projeto

*   Considerar diversas abordagens (soluções candidatas) que atenda um requisito e outro
*   Precisa ser rastreável entre os elementos de análise e os elementos de projeto
*   Utilizar padrões ao invés de reinventar a roda
*   Projeto precisa minimizar a distância entre o software e o mundo real (projeto que conecta os dois mundos)
*   Precisa ser estruturado para acomodar mudanças. É certo que o software vai mudar!
*   Precisa ser avaliado quanto a sua qualidade em cada etapa

### Conceitos de Projeto

1.  Abstração: sistema nasce num nível alto e desce até o código
2.  Refinamento: elaboração maior do nível de detalhes (complementar da abstração)
3.  Modularização: sistemas divididos em componentes
4.  Ocultação de Informações: sugere que cada módulo deve conter decisões de projeto. Modulo publica na interface só o que importa. Deve conter um segredo.

## Projetos de Software no RUP

Princípios essenciais do RUP

*   <span style="background-color: yellow;">-> Atacar os riscos de forma rápida e contínua</span>
*   Garantir que se está provendo algo de valor ao cliente
*   <span style="background-color: yellow;">-> Concentrar-se em produzir software executável</span>
*   <span style="background-color: yellow;">-> Acomodar mudanças no projeto</span>
*   <span style="background-color: yellow;">-> Definir a arquitetura o mais cedo possível</span>
*   <span style="background-color: yellow;">-> Construir o sistema com componentes</span>
*   Trabalhar em equipe
*   Fazer da qualidade uma forma de vida

<span style="background-color: yellow;">-> Impactam na etapa de projeto do sistema</span>  

*   Atacar os riscos: <span style="background-color: #ffe599;">RUP prega que devemos atacar primeiro os problemas que apresentam o maior risco para o sucesso do projeto.</span> É diferente do modelo em cascata nesse ponto. É preciso testar a arquitetura logo no inicio do projeto através de protótipos arquiteturais.
*   Construir o sistema com componentes: Componentes separam a interface da implementação. Possibilita a reutilização de partes. Reduz o impacto de mudanças.
*   Desenvolvimento iterativo e incremental
*   Fases e atividades do RUP

*   Concepção: entender o escopo e construir o caso de negócio

*   Objetivos:

*   Compreender o que construir
*   Identificar funcionalidades chave
*   Determinar ao menos uma solução possível 
*   Custos, prazos, riscos, qual processo, qual ferramentas
*   Decidir se deve continuar ou cancelar

*   Elaboração: reduzir os riscos técnicos, criar a arquitetura do sistema

*   Tem uma ou mais iterações, na primeira: Identificar cenários críticos, criar protótipos para testar esses cenários, fazer o projeto inicial do BD, detalhar os casos de uso de maior prioridade, validar arquitetura. Na segunda iteração, consertar problemas da primeira iteração, fechar projeto do BD, detalhar os casos de uso restantes, garantir que a arquitetura está estável.
*   Objetivos:

*   Detalhar os requisitos
*   Projetar, implementar e validar arquitetura
*   Mitigar os riscos principais
*   Revisar estimativas de prazo e custo
*   Refinar o processo
*   Implantar ferramentas

*   Construção: construir versão operacional do sistema
*   Transição: construir versão final do produto e entregar o cliente
*   Marcos: ao final de cada fase há marcos. 

### Arquitetura

#### Para projetar a arquitetura:

*   Componentes do sistema e suas interfaces
*   Decidir se cada componente será desenvolvido, reutilizado, comprado
*   Definir como os componentes vão interagir

#### Implementação

*   Criar protótipo arquitetural para validar a arquitetura
*   Projetar casos de uso críticos 
*   Consolidar e empacotar classes
*   Garantir uma cobertura arquitetural
*   Projetar BD
*   Identificar padrões
*   Delinear aspectos de concorrência e distribuição
*   Implementar cenários críticos
*   Integrar componentes
*   Testar cenários mais críticos

#### Protótipo arquitetural

<span style="background-color: yellow;">A arquitetura é definida com base nos casos de uso mais significativos.</span> Para se fazer um protótipo que represente bem a arquitetura do sistema, deve-se selecionar os casos de uso mais significativos pro sistema e desenvolver o protótipo em cima desses casos de uso.

#### Cobertura arquitetural

Garante que todos os elementos arquiteturais sejam cobertos através de um caso de uso.  

#### Validação arquitetura

Protótipo arquitetural tem que exibir as características adequadas.  

## Diagramas de Interação

Diagrama de Sequencia do Sistema - DSS

*   Ilustram as interações dos atores com o sistema
*   As operações iniciadas por eles
*   As respostas do sistema
*   É uma figura que mostra os eventos que os atores geram e a ordem que eles acontecem.
*   Deve ser feito um diagrama para a sequencia de sucesso e para cenários alternativos

**Modelagem Estrutural:** Diz respeitos de componentes que vão compor o sistema.**Modelagem Comportamental:** Ajuda projetar a lógica, comportamento do código, corpo dos métodos.  

Dois tipos de diagramas de interação:  

*   Diagrama de sequência: foi visto no vídeo
*   Diagrama de comunicação: apresentam as mensagens enfatizando relacionamentos.

Ambos são equivalentes.
