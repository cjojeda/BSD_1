drop database if exists tarea_Base_de_datos;
create database tarea_Base_de_datos;
use tarea_Base_de_datos;

drop table if exists agenda;
create table agenda(
nombre varchar(20),
domicilio varchar(30),
telefono varchar(11)
)ENGINE InnoDB;
 show tables; 
 describe agenda/*Descripcion de la tabla*/;
insert into agenda (nombre,domicilio,telefono) values("Weslry","Los Cedrales","0984444420");
insert into agenda (nombre,domicilio,telefono) values("Karen","CDE","0981347893");
insert into agenda (nombre,domicilio,telefono) values("Bianca","CDE","0982332505");
select * from agenda;
drop table if exists agenda;
drop table agenda;


/*------------------------------------------------------------*/
use tarea_Base_de_datos;
drop table if exists libros;
create table libros(
	titulo varchar(20),
	autor varchar(30),
	editorial varchar(15)
	);
SELECT * FROM libros;
insert into libros (titulo,autor,editorial)
values ('Abajo','José Ayala','Planeta');
show tables;
describe libros;
show tables;
describe libros;
drop table if exists libros;
drop table libors;