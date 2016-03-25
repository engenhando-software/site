title: "Mecanismos Arquiteturais"
date: 2015-10-04T11:04:00.000-03:00
updated: 2015-10-04T12:35:00.328-03:00
tags: 
- "disciplina2"
- "modulo3"
- "unidade3"
permalink: "mecanismos-arquiteturais"
comments: true
---

Permite que o arquiteto possa escolher tecnologias de forma correto no projeto.  

*   Um mecanismo arquitetural representa uma solução comum para um problema recorrente.
*   Um mecanismo liga requisitos arquiteturais a soluções técnicas, que podem ser expressas com a visão 4+1
*   Os requisitos do projeto influenciam os mecanismos de análise, desenho e implementação.

*   Mecanismos de analise: representa a solução independente de tecnologia
*   Mecanismos de desenho: a solução com algum viés tecnológico
*   Mecanismo de implementação: solução concreta

### Exemplo

Requisito arquitetural:

> Dados cadastrais devem estar disponíveis indefinidamente para consulta ou modificação.

Baseado nesse requisito, o <u>mecanismo de analise</u> seria a **persistência** dos dados, já que é uma solução comum no desenvolvimento de software.  

Já o <u>mecanismo de desenho</u>, influenciado pelo de análise, terá algum viés tecnológico, ele poderia por exemplo ser um **banco de dados relacional** ou um **arquivo de texto**, mas ainda não tem o nome da tecnologia em si.  

O <u>mecanismo de implementação</u> como terá uma solução concreta, esse requisito poderia ser implementado com o **MS SQLServer**.  

### Exemplo - Hotel ACME

Requisito arquitetural:  

> Usuários devem ser corretamente identificados

Restrições:  

*   A solução de segurança deve ser baseada em padrões abertos
*   As senhas não devem trafegar sobre a rede
*   A empresa já utiliza soluções Microsoft

Mecanismo de Análise  

*   Os projetistas estudam materiais técnicos sobre **autenticação** 
*   A autenticação é a solução técnica (padronizada) para credenciar usuários do sistema

Mecanismo de Desenho  

*   As soluções Kerberos e LDAP são elencadas, pois são padrões abertos
*   O Kerberos é escolhido, pois não trafega senhas sobre a rede.

Mecanismos de Implementação

*   Dado que a empresa já possui produtos MS, escolhemos um produto MS que suporta o protocolo Kerberos
*   Active Directory com Kerberos
