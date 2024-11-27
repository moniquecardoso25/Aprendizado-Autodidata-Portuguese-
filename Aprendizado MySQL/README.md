# Aprendizado MYSQL

## 1. Criar tabela
```sql
CREATE DATABASE learn
default character set uft8
default collate utf8_general_ci;

create table pessoas(
id int not null auto_increment,
nome varchar (30) not null,
nascimento date,
sexo enum('M','F'),
peso decimal (5,2),
altura decimal(3,2),
nacionalidade varchar(20) default 'Brasil',
primary key(id)
) default charset = uft8;
```

## 2. Inserir dados

```sql
use learn;
insert into pessoas 
(nome, nascimento, sexo, peso, altura, nacionalidade) 
values
("Márcia", "1985-03-28", "F", "78.5", "1.67", "Brasil");
```
