drop database if exists tarea_Base_de_datos;
create database tarea_Base_de_datos;
use tarea_Base_de_datos;
show databases;


create table autos(
  marca varchar(15),
  modelo year,
  dueño varchar(30),
  precio decimal (8,2) unsigned  
  )engine innodb;
insert into autos(marca,modelo,dueño,precio)
    values('Fiat 128','1970','Juan Lopez',50000);
insert into autos(marca,modelo,dueño,precio)
    values('Renault 11','1990','Juan Lopez',80000);
insert into autos(marca,modelo,dueño,precio)
    values('Fiat 128','1971','Ana Ferreyra',51000);
insert into autos(marca,modelo,dueño,precio)
    values('Peugeot 505','1998','Luis Luque',99000);
insert into autos(marca,modelo,dueño,precio)
    values('Peugeot 505','1997','Carola Perez',85000);

select * from autos
  where modelo<1995;
  
select marca,modelo from autos
  where modelo<>1970;

insert into autos(marca,modelo,dueño,precio)
    values('Peugeot 505',1995,'Carlos Lopez',88000); 


---------------------------- Segundo Problema ----------------------------

drop database if exists tarea_Base_de_datos;
create database tarea_Base_de_datos;
use tarea_Base_de_datos;
drop table if exists empleados;

create table empleados(
  nombre varchar(20),
  documento varchar(8),
  sexo char,
  domicilio varchar(30),
  fechaingreso date
 )engine innodb;
 
insert into empleados(nombre,documento,sexo,domicilio,fechaingreso)
  values('Juan Perez','22333444','m','Colon 123','1990-10-08');
insert into empleados(nombre,documento,sexo,domicilio,fechaingreso)
  values('Ana Acosta','23333444','f','Caseros 987','1995-12-18');
insert into empleados(nombre,documento,sexo,domicilio,fechaingreso)
  values('Lucas Duarte','25333444','m','Sucre 235','2005-05-15');
insert into empleados(nombre,documento,sexo,domicilio,fechaingreso)
  values('Pamela Gonzalez','26333444','f','Sarmiento 873','1999-02-12');
insert into empleados(nombre,documento,sexo,domicilio,fechaingreso)
  values('Marcos Juarez','30333444','m','Rivadavia 801','2002-09-22');

select nombre,fechaingreso from empleados
  where sexo = 'm';
update empleados set fechaingreso='1990-10-18'
  where documento='22333444';
insert into empleados(nombre,documento,sexo,domicilio,fechaingreso)
  values('Susana Duarte','30123456','f','Sucre 1234','99-02-12');

insert into empleados(nombre,documento,sexo,domicilio,fechaingreso)
  values('Daniel Herrero','30000001','m',null,'1980-2-03');

insert into empleados(nombre,documento,sexo,domicilio,fechaingreso)
  values('Ana Juarez','31123123','f',null,'19900306');

insert into empleados
  values('Juan Mores','32222333','m',null,'1990-03-06 10:15');


insert into empleados
  values('Hector Perez','34444555','m',null,'1990036');

