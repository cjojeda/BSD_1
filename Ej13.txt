-- Ejercicio 1
drop database if exists tarea_Base_de_datos;
create database tarea_Base_de_datos;
use tarea_Base_de_datos;

drop table if exists medicamentos;
create table medicamentos(
  codigo integer primary key auto_increment,
  nombre varchar(20),
  laboratorio varchar(20),
  precio float,
  cantidad integer
 );
 
  insert into medicamentos (nombre, laboratorio,precio,cantidad)
   values('Sertal','Roche',5.2,100);
 insert into medicamentos (nombre, laboratorio,precio,cantidad)
  values('Buscapina','Roche',4.10,200);
 insert into medicamentos (nombre, laboratorio,precio,cantidad)
  values('Amoxidal 500','Bayer',15.60,100);
  
  delete from medicamentos;
  
  insert into medicamentos (nombre, laboratorio,precio,cantidad)
   values('Sertal','Roche',5.2,100);
 insert into medicamentos (nombre, laboratorio,precio,cantidad)
  values('Amoxidal 500','Bayer',15.60,100);
  
  select * from medicamentos;
  
  truncate table medicamentos;
  insert into medicamentos (nombre, laboratorio,precio,cantidad)
  values('Buscapina','Roche',4.10,200);
  
    select * from medicamentos;
  
-- Ejercicio 2
drop database if exists tarea_Base_de_datos;
create database tarea_Base_de_datos;
use tarea_Base_de_datos;

drop table if exists peliculas;
create table peliculas (
codigo integer  primary key auto_increment,
titulo varchar (50),
actor varchar (40),
duracion integer

);

insert into peliculas (titulo,actor,duracion)
  values('Mision imposible','Tom Cruise',120);
 insert into peliculas (titulo,actor,duracion)
  values('Harry Potter y la piedra filosofal','xxx',180);
 insert into peliculas (titulo,actor,duracion)
  values('Harry Potter y la camara secreta','xxx',190);
 insert into peliculas (titulo,actor,duracion)
  values('Mision imposible 2','Tom Cruise',120);
 insert into peliculas (titulo,actor,duracion)
  values('La vida es bella','zzz',220);

truncate table peliculas;

insert into peliculas (titulo,actor,duracion)
  values('Mujer bonita','Richard Gere',120);

  select *from peliculas;
  
  truncate table peliculas;
insert into peliculas (titulo,actor,duracion)
  values('Elsa y Fred','China Zorrilla',90);
  
  select * from peliculas;
  
  