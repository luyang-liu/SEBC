* The first line of the server log
```
[root@ip-172-31-42-244 app]# more /var/log/cloudera-scm-server/cloudera-scm-server.log
2017-11-03 03:28:14,851 INFO main:com.cloudera.server.cmf.Main: Starting SCM Server. JVM Args: [-Dlog4j.configuration=file:/etc/cloudera-scm-server/log4j.properties, -Dfile.encoding=UTF-8, -D
cmf.root.logger=INFO,LOGFILE, -Dcmf.log.dir=/var/log/cloudera-scm-server, -Dcmf.log.file=cloudera-scm-server.log, -Dcmf.jetty.threshhold=WARN, -Dcmf.schema.dir=/usr/share/cmf/schema, -Djava.a
wt.headless=true, -Djava.net.preferIPv4Stack=true, -Dpython.home=/usr/share/cmf/python, -XX:+UseConcMarkSweepGC, -XX:+UseParNewGC, -XX:+HeapDumpOnOutOfMemoryError, -Xmx2G, -XX:MaxPermSize=256
m, -XX:+HeapDumpOnOutOfMemoryError, -XX:HeapDumpPath=/tmp, -XX:OnOutOfMemoryError=kill -9 %p], Args: [], Version: 5.13.0 (#55 built by jenkins on 20171002-1719 git: bd657e597e6743c458ee2c9aab
e808b7c972981c)


```
* The line(s) that contain the phrase "Started Jetty server"

```
2017-11-03 03:29:48,461 INFO WebServerImpl:com.cloudera.server.cmf.WebServerImpl: Started Jetty server.

```