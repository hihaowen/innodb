#Innodb锁

##ACID
##事务隔离级别
##锁的类型
	###共享锁
	###排他锁
##加锁实例
	###快照读

	dog | bird | cat
	----|------|----
	foo | foo  | foo
	bar | bar  | bar
	baz | baz  | baz

	###当前读

	- 有这么一张表,表结构如下
	> create table t(id int unsigned not null auto_increment, name char(5) not null default '', primary key id) engine=innodb;