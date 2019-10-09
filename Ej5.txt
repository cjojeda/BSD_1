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
  
  select * from peliculas;
  
  
 /*-----------------------------------------------------*/ 
use tarea_Base_de_datos;
drop table if exists empleados;
create table empleados (
	nombre varchar (20),
	documento varchar (8),
	sexo varchar (1),
	domicilio varchar(30),
	Sueldobasico float
	);
describe empleados;
insert into empleados (nombre, documento, sexo, domicilio, sueldobasico)values ('Juan Perez','22345678','m','Sarmiento 123',300);
insert into empleados (nombre, documento, sexo, domicilio, sueldobasico)values ('Ana Acosta','24345678','f','Colon 134',500); 
insert into empleados (nombre, documento, sexo, domicilio, sueldobasico)values ('Marcos Torres','27345678','m','Urquiza 479',800);
SELECT * FROM empleados;