
drop database if exists tarea_Base_de_datos;
create database tarea_Base_de_datos;
show databases;
use tarea_Base_de_datos;
drop table if exists autos;
create table autos(
  patente char(6)primary key not null,
  marca varchar(20),
  modelo char(4),
  precio float unsigned
 );
 

insert into autos (patente,marca,modelo,precio)
  values('ACD123','Fiat 128','1970',15000);
insert into autos (patente,marca,modelo,precio)
  values('ACG234','Renault 11','1990',40000);
insert into autos (patente,marca,modelo,precio)
  values('BCD333','Peugeot 505','1990',80000);
insert into autos (patente,marca,modelo,precio)
  values('GCD123','Renault Clio','1990',70000);
insert into autos (patente,marca,modelo,precio)
  values('BCC333','Renault Megane','1998',95000);
insert into autos (patente,marca,modelo,precio)
  values('BVF543','Fiat 128','1975',20000);
  
select * from autos 
   where modelo = '1990';
select * from autos
   where precio > 50000;
   

----------------------------------------------
drop database if exists tarea_Base_de_datos;
create database tarea_Base_de_datos;
use tarea_Base_de_datos;
drop table if exists clientes;

create table clientes(
  documento char(8) not null primary key,
  apellido varchar(20),
  nombre varchar(20),
  domicilio varchar(30),
  telefono varchar (11)
 )engine innodb;
 
insert into clientes (documento,apellido,nombre,domicilio,telefono)
  values('2233344','Perez','Juan','Sarmiento 980','4342345');
insert into clientes (documento,apellido,nombre,domicilio)
  values('2333344','Perez','Ana','Colon 234');
insert into clientes (documento,apellido,nombre,domicilio,telefono)
  values('2433344','Garcia','Luis','Avellaneda 1454','4558877');
insert into clientes (documento,apellido,nombre,domicilio,telefono)
  values('2533344','Juarez','Ana','Urquiza 444','4789900');
  
select * from clientes  where apellido = 'Perez';
select  apellido, domicilio , telefono from clientes where nombre =  'Ana';
    

