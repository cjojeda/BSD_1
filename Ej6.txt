drop database if exists tarea_Base_de_datos;
create database tarea_Base_de_datos;
use tarea_Base_de_datos;
 drop table if exists peliculas;
 create table peliculas(
  nombre varchar(20),
  actor varchar(20),
  duracion integer,
  cantidad integer
 );
describe peliculas;
insert into peliculas (nombre, actor, duracion, cantidad)
  values ('Mision imposible','Tom Cruise',120,3);
 insert into peliculas (nombre, actor, duracion, cantidad)
  values ('Mision imposible 2','Tom Cruise',180,2);
 insert into peliculas (nombre, actor, duracion, cantidad)
  values ('Mujer bonita','Julia R.',90,3);
 insert into peliculas (nombre, actor, duracion, cantidad)
  values ('Elsa y Fred','China Zorrilla',90,2);
  
  select nombre as "Titulo",actor as "Actor" from peliculas;
  select nombre as "Titulo" , duracion as "Duracion de la pelicula" from peliculas;
  select nombre as "Titulo" , cantidad as "Cantidad de copias" from peliculas;
  
  
  
  
/*-------------------------------------------------------*/  
  use tarea_Base_de_datos;
drop table agenda;
create table empleados(
	nombre varchar(20),  
	documento varchar(8), 
	sexo varchar(1),  
	domicilio varchar(30),
  	sueldobasico float
	)Engine Innodb;
insert into empleados (nombre, documento, sexo, domicilio, sueldobasico)	values ('Juan Perez','22345678','m','Sarmiento 123',300); 
insert into empleados (nombre, documento, sexo, domicilio, sueldobasico)     values ('Ana Acosta','24345678','f','Colon 134',500);
insert into empleados (nombre, documento, sexo, domicilio, sueldobasico)     values ('Marcos Torres','27345678','m','Urquiza 479',800);
select *from empleados;
select nombre,documento from empleados;
select nombre,documento,sueldobsico from empleados;




------------------------------------------- ----------------


  use tarea_Base_de_datos;
drop table articulos;
create table articulos(
codigo int, 
nombre varchar(20),
descripcion varchar(20),
precio float
	)Engine Innodb;
 
insert into articulos (codigo, nombre, descripcion, precio)  	values (1,'impresora','Epson Stylus C45',400.80);
 
insert into articulos (codigo, nombre, descripcion, precio)      values (2,'impresora','Epson Stylus C85',500);
 
insert into articulos (codigo, nombre, descripcion, precio)   	values (3,'monitor','Samsung 14',800);
  
select *from articulos;