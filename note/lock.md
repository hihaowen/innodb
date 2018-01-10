Innodb锁
========================

## ACID

## 事务隔离级别

## 锁的类型
 
 1. 共享锁
 2. 排他锁

## 加锁实例
 
 1. 快照读
 2. 当前读

 ### 有这么一张表,表结构如下

 > create table t(id int unsigned not null auto_increment, name char(5) not null default '', primary key (id)) engine=innodb;

| id | name  |
| -- | ----- |
|  1 | name1 |
|  2 | name2 |
|  3 | name3 |