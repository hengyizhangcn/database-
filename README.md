# database-review
数据库知识点记录

#1.常见的数据库有哪些
MySQL 轻量级，源码开放,  
SqlServer 微软公司, 
Oracle 甲骨文公司
DB2 IBM
Sybase
Sqlite

##分部式数据库:
(NoSQL, 非结构化)
MongoDB, HBase(和Hadoop关联), Cassandra(Facebook)
数据分片类型：水平分片，垂直分片，导出分片，混合分片
    分片条件：完备性条件，可重构条件，不相交条件
数据分配方式：集中式，分割式，全复制式，混合式

另：Redis，用于高速内存缓存数据应用

#2.数据库语言
##DDL 
create, alter, drop
eg.操作数据库
create database class;
drop database class;

eg. 操作表
以mysql为例
create table person(creidtId varchar(18) primary key, name text, age int, height int)

alter table person modify column height float
alter table person drop column height
alter table person add column height int

drop table person

##DQL
select
eg.
select * from person where age < 18

##DML
insert, update, delete
eg.
insert person values("12233219800512238X", "Michael", 15, 178)
update person set age = 20 where name = "Michael"
delete from person where creidtID = "12233219800512238X"

##DCL
grant, revoke，用于操作数据库
eg.
grant select/insert/update/delete/create/alter/drop/index/create view/references on person to users@micheal






Markdown: http://www.appinn.com/markdown/#p
