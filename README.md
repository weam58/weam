# weam
w
-- create database tvtc ;
______________________________________
create table dep (
depno int primary key ,
depname varchar(20)
);
______________________________________
create table std (
stdno int primary key ,
stdname varchar(20) ,
depno int ,
foreign key (depno) references dep(depno) );
_______________________________________
drop table dep ;
drop table std ;
alter table dep add loc varchar(20);
alter table dep drop column loc ;
alter table dep modify depname nvarchar(30);
