drop database if exists tarea_Base_de_datos;
create database tarea_Base_de_datos;
use tarea_Base_de_datos;

drop table if exists medicamentos;
create table medicamentos(
  codigo integer  primary key  auto_increment,
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
  
   select codigo,nombre,laboratorio,precio,cantidad
  from medicamentos;
  
  insert into medicamentos (codigo,nombre, laboratorio,precio,cantidad)
  values('12','Paracetamol 500','Bago',1.90,200);
  
  insert into medicamentos (nombre, laboratorio,precio,cantidad)
  values('Bayaspirina','Bayer',2.10,150); 

-- Ejercicio 2
drop database if exists tarea_Base_de_datos;
create database tarea_Base_de_datos;
use tarea_Base_de_datos;
drop table if exists peliculas;
create table peliculas ( codigo integer primary key  auto_increment,
 titulo varchar(30), 
 actor varchar(20), 
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
  
update peliculas set codigo='3' where actor ='Daniel R.';

delete from peliculas where titulo ='La vida es bella';

delete from trabajo_practico.peliculas where duracion = '120';

select * from peliculas;

insert into peliculas (titulo,actor,duracion)
  values('Mujer bonita','Richard Gere',120);
  
  insert into peliculas (codigo,titulo,actor,duracion)
  values('7','Tootsie','D. Hoffman',90);
  
  
 insert into peliculas (titulo,actor,duracion)
  values('Un oso rojo','Julio Chavez',100);

