
drop database if exists tarea_Base_de_datos;
create database tarea_Base_de_datos;
show databases;
use tarea_Base_de_datos;

create table pedidos(
  nro_pedido integer(3)  primary key auto_increment,
  nombre varchar(8),
  tipo varchar(20),
  precio decimal (2,2),
  cantidad integer(3),
  domicilio varchar(250)
  );

  
---------- Segundo Problema ----------

drop database if exists tarea_Base_de_datos;
create database tarea_Base_de_datos;
use tarea_Base_de_datos;
drop table estadisticas;

create table estadisticas(
    ciudad text,
    temperaturas int(3),
    precipitaciones_media_anual int(4) unsigned
    );
    
    
    
    
 -------------------------------------------
 
 drop database if exists tarea_Base_de_datos;
create database tarea_Base_de_datos;
use tarea_Base_de_datos;
drop table if exists gases;

create table gases(
    gas text,
    temperatura_critica decimal(3,1),
    presion_critica decimal(3,1) unsigned
);

drop table cuentas;

create table cuentas(
    nro_cuenta integer not null primary key,
    documento varchar(8) NOT NULL,
    nombre text,
    saldo_cuenta decimal (4,2)
);

