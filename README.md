# DBMS-Assignment
create database db;
use db;
create table project (Pid int primary key,Pname varchar(255),Startdate varchar(255),NoStudent int);
insert into project (Pid,Pname,Startdate,NoStudent) values(222,"HIG","28/07/2022",4);
insert into project (Pid,Pname,Startdate,NoStudent) values(212,"EFG","21/07/2022",3);
insert into project (Pid,Pname,Startdate,NoStudent) values(233,"ABC","22/07/2022",4);
insert into project (Pid,Pname,Startdate,NoStudent) values(144,"NOP","25/07/2022",5);
insert into project (Pid,Pname,Startdate,NoStudent) values(535,"KLM","24/07/2022",6);


alter table project add column Guidename varchar(255);



update project set Guidename="Shubhangi mam" where Pname="ABC";
update project set Guidename="Vairagar mam" where Pname="EFG";
update project set Guidename="Shubhangi mam" where Pname="HIG";
update project set Guidename="Vanita mam" where Pname="KLM";
update project set Guidename="Swati mam" where Pname="NOP";

select Pid,Pname,Startdate,NoStudent,Guidename from project order by Pid,Pname,Startdate,NoStudent,Guidename asc;

select * from project where Guidename = "Shubhangi mam";

select min(NoStudent) from project;

select sum(NoStudent) from project;
