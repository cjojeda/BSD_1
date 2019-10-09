drop database if exists tarea_Base_de_datos;
create database tarea_Base_de_datos;
use tarea_Base_de_datos;
drop table if exists libros;
 create table libros(
  codigo integer primary key not null,
  titulo varchar(50),
  autor varchar(30),
  editorial varchar(15)
 )engine innodb;
 describe libros;
     insert into libros(codigo,titulo,autor,editorial) values('1','El aleph','Borges','Planeta');
     insert into libros(codigo,titulo,autor,editorial) values('2','Martin Fierro','Jose Hernandez','Emece');
     insert into libros(codigo,titulo,autor,editorial) values('3','Aprenda PHP','Mario Molina','Emece');
     insert into libros(codigo,titulo,autor,editorial) values('4','Cervantes y el quijote','Borge','Paidos');
     insert into libros(codigo,titulo,autor,editorial) values('5','Matematica estas ahi','Paenza','Paidos');
     insert into libros(codigo,titulo,autor,editorial) values('6','NO se que libro','Paenza','Goku');
     insert into libros(codigo,titulo,autor,editorial) values('7','Matematica estas ahi','JohnCena','Paidos');
     insert into libros(codigo,titulo,autor,editorial) values('5','Matematica estas ahi','Goku','Paidos');

/*------------------2---------------*/



use tarea_Base_de_datos;
drop table if exists clientes;
create table clientes(
  documento varchar(8) primary key not null,
  apellido varchar(20),
  nombre varchar(20),
  domicilio varchar(30),
  telefono varchar (11)

 );
 
 insert into clientes (documento,apellido,nombre,domicilio, telefono)
   values('22345678','Perez','Marcos','Colon 123','4545454');
 insert into clientes (documento,apellido,nombre,domicilio, telefono)    
   values('23222222','Garcia','Ana','Avellaneda 1345','4252652');
 insert into clientes (documento,apellido,nombre,domicilio, telefono)   
   values('20454545','Lopez','Susana','Urquiza 344','4522525');
 insert into clientes (documento,apellido,nombre,domicilio, telefono)   
   values('35454545','Lopez','Susana','Urquiza 344','4522525');
   
   insert into clientes (documento,apellido,nombre,domicilio, telefono)
   values('22345679','Perez','Marcos','Colon 1234','45454954');
  insert into clientes (documento,apellido,nombre,domicilio, telefono)
  values('248615','Vidal','Melgarejo','Colon 1234','454554954'); 
   
   
 insert into clientes (documento,apellido,nombre,domicilio, telefono)
  values('248615','Vidal','Melgarejo','Colon 1234','454554954'); 

/*--------------------------3--------------------------------*/

use tarea_Base_de_datos;
drop table if exists alumnos;

create table alumnos(
  legajo varchar(4) primary key not null,
  documento varchar(8) not null,
  apellido varchar(30),
  nombre varchar(30),
  domicilio varchar(30)
 );
 
 insert into alumnos (legajo,documento,apellido,nombre,domicilio)
  values('A233','22345345','Perez','Mariana','Colon 234');
 insert into alumnos (legajo,documento,apellido,nombre,domicilio)
  values('A567','23545345','Morales','Marcos','Avellaneda 348');
 insert into alumnos (legajo,documento,apellido,nombre,domicilio)
  values('B654','24356345','Gonzalez','Analia','Caseros 444');
 insert into alumnos (legajo,documento,apellido,nombre,domicilio)
  values('A642','20254125','Torres','Ramiro','Dinamarca 209');
 insert into alumnos (legajo,documento,apellido,nombre,domicilio)
  values('B509','20445778','Miranda','Carmen','Uspallata 999');
 insert into alumnos (legajo,documento,apellido,nombre,domicilio)
  values('C777','28111444','Figueroa','Natalia','Sarmiento 856');
  
  
  Select * from alumnos;
  
  insert into alumnos (legajo,documento,apellido,nombre,domicilio)
  values('C778','28111444','Vidal','Melgarejo','Sarmiento 859'); 
  insert into alumnos (legajo,documento,apellido,nombre,domicilio)
  values('C777','28111444','Figueroa','Natalia','Sarmiento 856'); 

