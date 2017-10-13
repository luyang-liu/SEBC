* The first line of the server log
```
[root@ip-172-31-40-116 cloudera-scm-server]# more cloudera-scm-server.log
2017-10-13 02:13:54,557 INFO main:com.cloudera.server.cmf.Main: Starting SCM Server. JVM Args: [-Dlog4j.configuration=file:/etc/cloudera-scm-server/log4j.properties, -Dfile.encoding=UTF-8, -D
cmf.root.logger=INFO,LOGFILE, -Dcmf.log.dir=/var/log/cloudera-scm-server, -Dcmf.log.file=cloudera-scm-server.log, -Dcmf.jetty.threshhold=WARN, -Dcmf.schema.dir=/usr/share/cmf/schema, -Djava.a
wt.headless=true, -Djava.net.preferIPv4Stack=true, -Dpython.home=/usr/share/cmf/python, -XX:+UseConcMarkSweepGC, -XX:+UseParNewGC, -XX:+HeapDumpOnOutOfMemoryError, -Xmx2G, -XX:MaxPermSize=256
m, -XX:+HeapDumpOnOutOfMemoryError, -XX:HeapDumpPath=/tmp, -XX:OnOutOfMemoryError=kill -9 %p], Args: [], Version: 5.10.2 (#9 built by jenkins on 20170626-1942 git: 15f547c8802e02d59901ee3fe1c
5c5733eab0227)

```
* The line(s) that contain the phrase "Started Jetty server"

```
2017-10-13 02:15:53,481 INFO WebServerImpl:com.cloudera.server.cmf.WebServerImpl: Started Jetty server.

```