
-- Ejercicio 1
drop database if exists tarea_Base_de_datos;
create database tarea_Base_de_datos;
use tarea_Base_de_datos;
drop table if exists medicamentos;

create table medicamentos(
  codigo integer auto_increment   primary key,
  nombre varchar(20) not null,
  laboratorio varchar(20),
  precio float,
  cantidad integer not null
 )engine innodb;
 
 select * from medicamentos;
 
 insert into medicamentos (nombre,laboratorio,precio,cantidad)
  values('Sertal gotas','Roche',5.2,100); 
 insert into medicamentos (nombre,laboratorio,precio,cantidad)
  values('Sertal compuesto','Roche',7.1,150);
 insert into medicamentos (nombre,laboratorio,precio,cantidad)
  values('Buscapina','Roche',null,200);
 insert into medicamentos (nombre,laboratorio,precio,cantidad)
  values('Amoxidal 500','Bayer',15.60,0);
 insert into medicamentos (nombre,laboratorio,precio,cantidad)
  values('Amoxidal jarabe','Bayer',25,120);
 insert into medicamentos (nombre,laboratorio,precio,cantidad)
  values('Amoxinil',null,25,120);
 insert into medicamentos (nombre, laboratorio,precio,cantidad)
  values('Bayaspirina','',0,150); 
  
   select * from medicamentos where laboratorio is null;
   
    select * from medicamentos where laboratorio='';
    
    select * from medicamentos where precio is null;
  select * from medicamentos where precio=0;
  
  insert into medicamentos (nombre, laboratorio,precio,cantidad)
  values(null,'Bayer',10.20,100);
  
  insert into medicamentos (nombre, laboratorio,precio,cantidad)
  values('Benadryl comprimidos','Bayer',10.20,null); 
  
  insert into medicamentos (codigo,nombre, laboratorio,precio,cantidad)
  values(null,'Benadryl comprimidos','Bayer',10.20,null);
  
  select * from medicamentos where precio<>0;
 select * from medicamentos where precio is not null;
 
 select * from medicamentos where precio<>0;
 select * from medicamentos where precio is not null;
 
-- Ejercicio 2


drop database if exists tarea_Base_de_datos;
create database tarea_Base_de_datos;
use tarea_Base_de_datos;
drop table if exists peliculas;
create table peliculas (
codigo integer auto_increment primary key,
titulo varchar (30) not null,
actor varchar (20),
duracion integer
)engine innodb;
select * from peliculas;

insert into peliculas (titulo,actor,duracion)
  values('Mision imposible','Tom Cruise',120);
 insert into peliculas (titulo,actor,duracion)
  values('Harry Potter 1','Daniel R.',180);
 insert into peliculas (titulo,actor,duracion)
  values('Harry Potter 2','Daniel R.',190);
 insert into peliculas (titulo,actor,duracion)
  values('Mision imposible 2','Tom Cruise',150);
 insert into peliculas (titulo,actor,duracion)
  values('Titanic','L. Di Caprio',220);
 insert into peliculas (titulo,actor,duracion)
  values('Mujer bonita','R. Gere-J. Roberts',200);

insert into peliculas (codigo,titulo,actor,duracion)
  values(null,'Elsa y Fred','China Zorrilla',90);
  
  insert into peliculas (titulo,actor,duracion)
  values('Mr. Johns',null,null);
  
  insert into peliculas (codigo,titulo,actor,duracion)
  values(0,'','',0);
  
  update peliculas set duracion=120 where duracion is null;
  update peliculas set actor='Desconocido'
  where actor is null;
  
  update peliculas set actor='Desconocido'
  where actor='';
