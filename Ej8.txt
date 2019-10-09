
drop database if exists tarea_Base_de_datos;
create database tarea_Base_de_datos;
use tarea_Base_de_datos;
drop table if exists articulos;
  create table articulos(
  codigo integer,
  nombre varchar(20),
  descripcion varchar(30),
  precio float,
  cantidad integer
 )engine innoDB;
 
 insert into articulos (codigo, nombre, descripcion, precio,cantidad)values (1,'impresora','Epson Stylus C45',400.80,20);
 insert into articulos (codigo, nombre, descripcion, precio,cantidad)values (2,'impresora','Epson Stylus C85',500,30);
 insert into articulos (codigo, nombre, descripcion, precio,cantidad)  values (3,'monitor','Samsung 14',800,10);
 insert into articulos (codigo, nombre, descripcion, precio,cantidad)values (4,'teclado','ingles Biswal',100,50);
 insert into articulos (codigo, nombre, descripcion, precio,cantidad) values (5,'teclado','español Biswal',90,50);
select *  from articulos;
select * from articulos where precio>=500;
select *from articulos where cantidad<30;
select nombre, descripcion from articulos  where precio<>100;



----------------------------------------- ----


use tarea_Base_de_datos;
drop table if exists peliculas;
create table peliculas(
  titulo varchar(20),
  actor varchar(20),
  duracion integer,
  cantidad integer
 )engine Innodb;


insert into peliculas (titulo, actor, duracion, cantidad)

	values ('Mision imposible','Tom Cruise',120,3);

insert into peliculas (titulo, actor, duracion, cantidad)

	values ('Mision imposible 2','Tom Cruise',180,2);

insert into peliculas (titulo, actor, duracion, cantidad)

	values ('Mujer bonita','Julia R.',90,3);
 
insert into peliculas (titulo, actor, duracion, cantidad)

	values ('Elsa y Fred','China Zorrilla',90,2);


select *from peliculas

	where duracion<=90;

select * from peliculas

	where actor<>'Tom Cruise';

select * from peliculas

	where cantidad >2;

------------------- -------------------

use tarea_Base_de_datos;


drop table if exists agenda;
create table agenda(

	apellido varchar(20),

	nombre varchar(20),

	domicilio varchar(30),

	telefono varchar(11)

	)engine innodb;
 


insert into agenda(apellido,nombre,domicilio,telefono)
	values('Mores','Alberto','Colon 123','4234567');

insert into agenda(apellido,nombre,domicilio,telefono)
	values('Torres','Juan','Avellaneda 135','4458787'); 
insert into agenda(apellido,nombre,domicilio,telefono)
	values('Lopez','Mariana','Urquiza 333','4545454');

insert into agenda(apellido,nombre,domicilio,telefono)
	values('Lopez','Fernando','Urquiza 333','4545454');
 
insert into agenda(apellido,nombre,domicilio,telefono)
	values('Suarez','Mariana','Sarmiento 643','4445544');

insert into agenda(apellido,nombre,domicilio,telefono)
	values('Lopez','Ana','Sucre 309','4252587');


select * from agenda;


select * from agenda
	where apellido='Lopez';


select * from agenda 
	where nombre<>'Mariana';


select * from agenda 
	where domicilio='Colon 123';


select * from agenda 
	where telefono='4545454';