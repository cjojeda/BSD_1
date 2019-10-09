drop database if exists tarea_Base_de_datos;
create database tarea_Base_de_datos;
use tarea_Base_de_datos;

drop table agenda; 
drop table if exists agenda;

create table agenda(
nombre varchar(20),
domicilio varchar(30),
telefono varchar(11)

)ENGINE InnoDB;

create table agenda;

 show tables;

 describe agenda;

drop table if exists agenda;
/*-----------------------------------------------*/
use tarea_Base_de_datos;
drop table if exists libros;
create table libros(

	titulo varchar(20),

	autor varchar(30),

	editorial varchar(15)

	)ENGINE InnoDB;

show tables;
describe libros;
 drop table if exists libros;
 drop table libros;

