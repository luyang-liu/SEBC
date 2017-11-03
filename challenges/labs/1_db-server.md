﻿* The command  hostname -f  and its output :  
```
[root@ip-172-31-40-179 app]# hostname -f
ip-172-31-40-179.us-west-2.compute.internal
```
* The command  mysql -u <user> -p<password> -e "status;"  and its output
``` 
[root@ip-172-31-40-179 app]# mysql -u root -pneusoft -e "status;"
--------------
mysql  Ver 14.14 Distrib 5.5.58, for Linux (x86_64) using readline 5.1

Connection id:		11
Current database:	
Current user:		root@localhost
SSL:			Not in use
Current pager:		stdout
Using outfile:		''
Using delimiter:	;
Server version:		5.5.58-log MySQL Community Server (GPL)
Protocol version:	10
Connection:		Localhost via UNIX socket
Server characterset:	latin1
Db     characterset:	latin1
Client characterset:	utf8
Conn.  characterset:	utf8
UNIX socket:		/var/lib/mysql/mysql.sock
Uptime:			5 min 20 sec

Threads: 1  Questions: 48  Slow queries: 0  Opens: 34  Flush tables: 1  Open tables: 27  Queries per second avg: 0.150
--------------

```
* The command  mysql -u <user> -p<password> -e "show databases;"  and its output
```
[root@ip-172-31-40-179 app]# mysql -u root -pneusoft -e "show databases;"
+--------------------+
| Database           |
+--------------------+
| information_schema |
| hive               |
| hue                |
| mysql              |
| oozie              |
| performance_schema |
| rman               |
| scm                |
| sentry             |
+--------------------+


```
