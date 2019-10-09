drop database if exists tarea_Base_de_datos;
create database tarea_Base_de_datos;
use tarea_Base_de_datos;
  drop table if exists agenda;
create table agenda(
nombre varchar(20),
domicilio varchar(30),
telefono varchar(11)
)ENGINE InnoDB;
 describe agenda;
insert into agenda(nombre,domicilio,telefono) values ( 'Alberto Mores','Colon 123','4234567');
insert into agenda(nombre,domicilio,telefono) values ('Juan Torres','Avellaneda 135','4458787');
insert into agenda(nombre,domicilio,telefono) values ('Mariana Lopez','Urquiza 333','4545454');
insert into agenda(nombre,domicilio,telefono) values ('Fernando Lopez','Urquiza 333','4545454');
select * from agenda;
select * from agenda where nombre = "Juan Torres";
select * from agenda where domicilio = "Colon 123";
 drop table agenda;
 ----------------------------- --------------------------------
 

use tarea_Base_de_datos;
drop table if exists libros;
create table libros(

	titulo varchar(20),

	autor varchar(30),

	editorial varchar(15)

	)Engine Innodb;



insert into libros(titulo,autor,editorial) 
	values ('El aleph','Borges','Planeta');

insert into libros(titulo,autor,editorial) 
	values ('Martin Fierro','Jose Hernandez','Emece');

insert into libros(titulo,autor,editorial) 
	values ('Aprenda PHP','Mario Molina','Emece');

insert into libros(titulo,autor,editorial) 
	values ('Cervantes','Borges','Paidos');


select *from libros;


select *from libros 
	where autor='Borges';

select *from libros 
	where editorial='Emece';

select *from libros 
	where titulo='Martin Fierro';



drop table libros;

-------------- Tercer Problema --------------

use tarea_Base_de_datos;

drop tables if exists articulos;

create table articulos(

	codigo integer,
  
	nombre varchar(20),
  
	descripcion varchar(30),
  
	precio float
 )Engine InnoDB;
 
  

insert into articulos (codigo, nombre, descripcion, precio)
  
	values (1,'impresora','Epson Stylus C45',400.80);
 
insert into articulos (codigo, nombre, descripcion, precio)
  
	values (2,'impresora','Epson Stylus C85',500);
 
insert into articulos (codigo, nombre, descripcion, precio)
  
	values (3,'monitor','Samsung 14',800);
 
insert into articulos (codigo, nombre, descripcion, precio)
  
	values (4,'teclado','ingles Biswal',100);
 
insert into articulos (codigo, nombre, descripcion, precio)
  
	values (5,'teclado','español Biswal',90);

  
  
select *from articulos 
	where nombre='impresora';
  

select codigo,descripcion,precio from articulos;

