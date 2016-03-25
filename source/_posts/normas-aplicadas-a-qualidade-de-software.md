title: "Normas Aplicadas a Qualidade de Software"
date: 2015-04-29T23:02:00.000-03:00
updated: 2015-09-07T16:09:02.482-03:00
tags: 
- "disciplina1"
- "modulo2"
- "unidade3"
permalink: "normas-aplicadas-a-qualidade-de-software"
comments: true
---

## ISO 9126

Define características e sub-características. Norma técnica sempre te dá o roteiro sobre "o que fazer" e não como.Define um conjunto de 6 visões da qualidade para produtos de software:

1.  **Funcionalidade**: entender quais as funções;

*   **Adequação**: medir o tanto que o software é adequado aos processos do cliente (mais usada)
*   **Acurácia**: precisão, saber se o software entrega dados corretos e precisos
*   **Interoperabilidade**: capacidade que o sistema tem de integrar com outros sistemas
*   **Conformidade**: os dados gerados pelo sistema estão de acordo com as regras do negócio. Ex. Calculo do imposto de renda, está fiel ao calculo do IR?
*   **Segurança**: saber se o sistema evita acessos não autorizados

3.  **Confiabilidade**: o esforço de medir as indisponibilidades do sistemas, diz respeito a falhas

*   **Maturidade**: frequência de falhas, quanto maior o numero de falhas, menos maduro
*   **Tolerância a falhas**: robustez do sistema. Reage bem após falha.
*   **Recuperabilidade**: capacidade de recuperar dados, transações pós falha.
*   **Conformidade**: Não estar em conformidade com o contrato redigido pelo cliente.

5.  **Usabilidade**: esforço de uso do sistema

*   **Inteligibilidade**: capacidade que o sistema tem de passar para o usuário o seu propósito.
*   **Apreensibilidade**: esforço de uso do sistema.
*   **Atratividade**: capacidade de atração que proporciona ao usuário.
*   **Operatividade**: instalação do software, colocar disponível, fazer backup, etc. 
*   **Conformidade**: se está em conformidade com padrões de organização, fonte, etc.

7.  **Eficiência**: desempenho

*   **Comportamento em relação ao tempo**: quanto tempo leva para o sistema te retornar uma informação. 
*   **Comportamento em relação aos recursos**: recursos é memória, CPU, etc. 
*   **Conformidade**: sistema tem entregue dentro de uma eficiência acordada (contrato).

9.  **Manutenibilidade**: esforço de manutenção

*   **Analisibilidade**: esforço de analisar aonde existe algum problema a ser resolvido. Quanto menor o esforço de analisar o sistema, melhor.
*   **Modificabilidade**: esforço de modificação do código.
*   **Estabilidade**: risco de se mexer no sistema.
*   **Testabilidade**: esforço de teste após manutenção.
*   **Conformidade**: mesmo das outras características, está sendo feita dentro do que foi acordado.

11.  **Portabilidade**: capacidade que o sistema tem de trabalhar em diferentes ambientes operacionais

*   **Adaptabilidade**: o quanto que o sistema se adapta ao ambiente especificado (Win, Linux)
*   **Coexistência**: capacidade de coexistir com outros softwares.
*   **Capacidade para ser instalado:** qual o esforço para instalar num ambiente ou no outro.
*   **Capacidade para substituir:** capacidade de substituir um outro sistema num outro ambiente. Ex. Office no Windows -> não tem capacidade de substituir outro pacote de escritório no linux
*   **Conformidade**: portabilidade acordada para o software está sendo atendida?

### Sistema quantitativo para medir qualidade

> Qualidade de Software = soma(características)  
> Características = soma(subcaracteristicas)  
> Subcaracterísitcas = soma(métricas)

_<span style="background-color: yellow;">Métricas são perguntas objetivas</span> feitas para o avaliador responder sobre o sistema__<span style="background-color: yellow;">Peso é um valor relativo da importância que se atribui</span> <span style="background-color: white;">a cada uma característica</span>. Ex. sistema web deve ter um peso maior para Usabilidade. Automação deve ter um peso maior na confiabilidade._

## ISO 14598

Trata o processo de avaliação do software. Bem mais recente que a ISO 9126\. É um roteiro de como projetar uma avaliação de um software.Possui 4 momentos:

1.  Estabelecer requisitos de avaliação: 

*   estabelecer o proposito da avaliação
*   identificar o tipo de produto a ser avaliado
*   especificar um modelo de qualidade (ISO 9126)

3.  Especificar a avaliação

*   selecionar métricas (criar métricas para as características)
*   atribuir valores/pesos para as métricas
*   estabelecer critérios para julgamento

5.  Projetar a avaliação (fazer o plano de avaliação)

*   plano deve conter métricas para ser avaliados por usuários, desenvolvedores, etc. cada um no que entende. Ex. desenvolvedor que avalia a confiabilidade, e o usuário que avalia a usabilidade.

7.  Executar a avaliação

*   obter as medidas
*   comparar com critérios
*   julgar os resultados
