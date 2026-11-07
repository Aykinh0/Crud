create database bd_crudtp;
use bd_crudtp;

create table if not exists tb_aluno(
cd_aluno int not null auto_increment,
cd_rm_aluno char(7),
nm_aluno varchar(60),
nr_idade_aluno tinyint unsigned not null,
email_aluno varchar(120) not null unique,
senha_aluno varchar(20),
constraint pk_aluno_cadastro
	primary key(cd_aluno))
engine InnoDB;

select * from tb_aluno;
