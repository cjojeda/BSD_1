-- Ejercicio 1
drop database if exists tarea_Base_de_datos;
create database tarea_Base_de_datos;
use tarea_Base_de_datos;
drop table if exists peliculas;
create table peliculas(
  codigo integer unsigned primary key auto_increment,
  titulo varchar(40) not null,
  actor varchar(20),
  duracion integer unsigned
 );

-- Ejercicio 2

drop database if exists tarea_Base_de_datos;
create database tarea_Base_de_datos;
use tarea_Base_de_datos;
drop table if exists visistantesp;
create table visitantes (
nombre varchar (30),
edad integer,
sexo char,
domicilio varchar (30),
cuidad varchar (30),
telefono varchar (11),
monto float

);

select * from visitantes;

