drop database if exists tarea_Base_de_datos;
create database tarea_Base_de_datos;
show databases;
use tarea_Base_de_datos;
drop table if exists peliculas;

create table peicula(
    codigo int unsigned auto_increment primary key,
    titulo varchar(50) NOT NULL,
    actor varchar(20),
    duracion int unsigned
    )engine innodb;

insert into peliculas (titulo,actor,duracion)values('Mision imposible','Tom Cruise',120);  
insert into peliculas (codigo,duracion)values(5,90);

insert into peliculas (titulo,actor)values ('Harry Potter y la piedra filosofal','Daniel R.');
insert into peliculas (titulo,actor,duracion)values ('Harry Potter y la piedra filosofal','Daniel R.',120);
  
select * from pelicula;




-----------------------------------------------------------
drop database if exists tarea_Base_de_datos;
create database tarea_Base_de_datos;
show databases;
use tarea_Base_de_datos;
drop table if exists empleados;

create table empleados(
  nombre varchar(20),
  documento varchar(8) NOT NULL,
  sexo char,
  domicilio varchar(30),
  fechaingreso date NOT NULL,
  fechanacimiento date,
  sueldo decimal(5,2) unsigned NOT NULL
  )engine innodb;

insert into empleados (nombre,documento,sexo)values('Marcela Medina','22333444','f');
insert into empleados (domicilio,fechaingreso)values('Avellaneda 200','2005-08-16');
insert into empleados (fechanacimiento,sueldo)values('1970-09-26',500.90);
select * from empleados;