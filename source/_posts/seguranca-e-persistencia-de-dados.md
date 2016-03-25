title: "Segurança e Persistência de Dados"
date: 2015-03-05T22:15:00.000-03:00
updated: 2015-06-06T15:56:12.761-03:00
tags: 
- "disciplina4"
- "modulo1"
- "unidade3"
permalink: "seguranca-e-persistencia-de-dados"
comments: true
---

Dois tipos de segurança  

*   Segurança de Acesso  (acesso ao dado)
*   Segurança de Atualização (não é atualização do dado, é a persistência do dado)

### Segurança de Acesso

Dois tipos de privilégio

*   Nível de conta: relacionado ao usuário do banco de dados, esse usuário pode criar uma tabela, uma view, etc. (DDL)
*   Nivel de relação(tabela ou view): select, insert, update, delete, alter table, index, etc (DML)

*   grant select, insert, delete on TABELA to USER or ROLE
*   revoke select, insert, ... on TABELA to USER or ROLE
*   grant option permite o usuario dar permissões a outros

### Segurança de Atualização

É a segurança que o usuário tem em manter o dado persistido, se ele assim o quiser.  

*   Commit 
*   Rollback
*   Log
*   Backup full, incremental
*   Recover (time stamp)

É o backup, recovery e log do banco de dadosrecovery = backupFull + Soma(BackupIncrementais) + Log
