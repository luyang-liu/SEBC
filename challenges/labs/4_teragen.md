* The full  teragen  command and output
```
[reilly@ip-172-31-36-244 ~]$ time hadoop jar /opt/cloudera/parcels/CDH/jars/hadoop*-examples.jar teragen -Dmapred.map.tasks=12 -Ddfs.block.size=33554432 -Dmapreduce.map.memory.mb=1024 65536000  /user/reilly/tgen
17/11/03 04:20:59 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-42-244.us-west-2.compute.internal/172.31.42.244:8032
17/11/03 04:20:59 INFO terasort.TeraSort: Generating 65536000 using 12
17/11/03 04:20:59 INFO mapreduce.JobSubmitter: number of splits:12
17/11/03 04:20:59 INFO Configuration.deprecation: mapred.map.tasks is deprecated. Instead, use mapreduce.job.maps
17/11/03 04:20:59 INFO Configuration.deprecation: dfs.block.size is deprecated. Instead, use dfs.blocksize
17/11/03 04:21:00 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1509681772775_0001
17/11/03 04:21:00 INFO impl.YarnClientImpl: Submitted application application_1509681772775_0001
17/11/03 04:21:00 INFO mapreduce.Job: The url to track the job: http://ip-172-31-42-244.us-west-2.compute.internal:8088/proxy/application_1509681772775_0001/
17/11/03 04:21:00 INFO mapreduce.Job: Running job: job_1509681772775_0001
17/11/03 04:21:08 INFO mapreduce.Job: Job job_1509681772775_0001 running in uber mode : false
17/11/03 04:21:08 INFO mapreduce.Job:  map 0% reduce 0%
17/11/03 04:21:21 INFO mapreduce.Job:  map 4% reduce 0%
17/11/03 04:21:22 INFO mapreduce.Job:  map 10% reduce 0%
17/11/03 04:21:23 INFO mapreduce.Job:  map 12% reduce 0%
17/11/03 04:21:24 INFO mapreduce.Job:  map 17% reduce 0%
17/11/03 04:21:25 INFO mapreduce.Job:  map 19% reduce 0%
17/11/03 04:21:26 INFO mapreduce.Job:  map 22% reduce 0%
17/11/03 04:21:27 INFO mapreduce.Job:  map 24% reduce 0%
17/11/03 04:21:28 INFO mapreduce.Job:  map 25% reduce 0%
17/11/03 04:21:29 INFO mapreduce.Job:  map 27% reduce 0%
17/11/03 04:21:30 INFO mapreduce.Job:  map 29% reduce 0%
17/11/03 04:21:31 INFO mapreduce.Job:  map 30% reduce 0%
17/11/03 04:21:32 INFO mapreduce.Job:  map 33% reduce 0%
17/11/03 04:21:33 INFO mapreduce.Job:  map 35% reduce 0%
17/11/03 04:21:35 INFO mapreduce.Job:  map 38% reduce 0%
17/11/03 04:21:36 INFO mapreduce.Job:  map 39% reduce 0%
17/11/03 04:21:37 INFO mapreduce.Job:  map 40% reduce 0%
17/11/03 04:21:38 INFO mapreduce.Job:  map 42% reduce 0%
17/11/03 04:21:39 INFO mapreduce.Job:  map 44% reduce 0%
17/11/03 04:21:40 INFO mapreduce.Job:  map 45% reduce 0%
17/11/03 04:21:41 INFO mapreduce.Job:  map 47% reduce 0%
17/11/03 04:21:42 INFO mapreduce.Job:  map 48% reduce 0%
17/11/03 04:21:43 INFO mapreduce.Job:  map 49% reduce 0%
17/11/03 04:21:45 INFO mapreduce.Job:  map 51% reduce 0%
17/11/03 04:21:46 INFO mapreduce.Job:  map 52% reduce 0%
17/11/03 04:21:47 INFO mapreduce.Job:  map 53% reduce 0%
17/11/03 04:21:48 INFO mapreduce.Job:  map 56% reduce 0%
17/11/03 04:21:49 INFO mapreduce.Job:  map 57% reduce 0%
17/11/03 04:21:50 INFO mapreduce.Job:  map 58% reduce 0%
17/11/03 04:21:51 INFO mapreduce.Job:  map 61% reduce 0%
17/11/03 04:21:52 INFO mapreduce.Job:  map 62% reduce 0%
17/11/03 04:21:53 INFO mapreduce.Job:  map 64% reduce 0%
17/11/03 04:21:54 INFO mapreduce.Job:  map 65% reduce 0%
17/11/03 04:21:55 INFO mapreduce.Job:  map 66% reduce 0%
17/11/03 04:21:56 INFO mapreduce.Job:  map 69% reduce 0%
17/11/03 04:21:57 INFO mapreduce.Job:  map 70% reduce 0%
17/11/03 04:21:59 INFO mapreduce.Job:  map 73% reduce 0%
17/11/03 04:22:00 INFO mapreduce.Job:  map 74% reduce 0%
17/11/03 04:22:01 INFO mapreduce.Job:  map 75% reduce 0%
17/11/03 04:22:02 INFO mapreduce.Job:  map 77% reduce 0%
17/11/03 04:22:03 INFO mapreduce.Job:  map 78% reduce 0%
17/11/03 04:22:04 INFO mapreduce.Job:  map 79% reduce 0%
17/11/03 04:22:05 INFO mapreduce.Job:  map 80% reduce 0%
17/11/03 04:22:06 INFO mapreduce.Job:  map 82% reduce 0%
17/11/03 04:22:08 INFO mapreduce.Job:  map 84% reduce 0%
17/11/03 04:22:09 INFO mapreduce.Job:  map 86% reduce 0%
17/11/03 04:22:10 INFO mapreduce.Job:  map 87% reduce 0%
17/11/03 04:22:11 INFO mapreduce.Job:  map 90% reduce 0%
17/11/03 04:22:13 INFO mapreduce.Job:  map 92% reduce 0%
17/11/03 04:22:14 INFO mapreduce.Job:  map 93% reduce 0%
17/11/03 04:22:16 INFO mapreduce.Job:  map 95% reduce 0%
17/11/03 04:22:17 INFO mapreduce.Job:  map 96% reduce 0%
17/11/03 04:22:19 INFO mapreduce.Job:  map 97% reduce 0%
17/11/03 04:22:20 INFO mapreduce.Job:  map 99% reduce 0%
17/11/03 04:22:21 INFO mapreduce.Job:  map 100% reduce 0%
17/11/03 04:22:23 INFO mapreduce.Job: Job job_1509681772775_0001 completed successfully
17/11/03 04:22:24 INFO mapreduce.Job: Counters: 31
	File System Counters
		FILE: Number of bytes read=0
		FILE: Number of bytes written=1469174
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=1025
		HDFS: Number of bytes written=6553600000
		HDFS: Number of read operations=48
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=24
	Job Counters 
		Launched map tasks=12
		Other local map tasks=12
		Total time spent by all maps in occupied slots (ms)=586131
		Total time spent by all reduces in occupied slots (ms)=0
		Total time spent by all map tasks (ms)=586131
		Total vcore-seconds taken by all map tasks=586131
		Total megabyte-seconds taken by all map tasks=600198144
	Map-Reduce Framework
		Map input records=65536000
		Map output records=65536000
		Input split bytes=1025
		Spilled Records=0
		Failed Shuffles=0
		Merged Map outputs=0
		GC time elapsed (ms)=2112
		CPU time spent (ms)=152700
		Physical memory (bytes) snapshot=4209307648
		Virtual memory (bytes) snapshot=18766204928
		Total committed heap usage (bytes)=4460118016
	org.apache.hadoop.examples.terasort.TeraGen$Counters
		CHECKSUM=140750829423462787
	File Input Format Counters 
		Bytes Read=0
	File Output Format Counters 
		Bytes Written=6553600000

real	1m27.632s
user	0m6.003s
sys	0m0.649s


```
* The result of the  time  command
```
real	1m27.632s
user	0m6.003s
sys	0m0.649s
```
* The command and output of  hdfs dfs -ls /user/reilly/tgen
```
[reilly@ip-172-31-36-244 ~]$ hdfs dfs -ls /user/reilly/tgen
Found 13 items
-rw-r--r--   3 reilly supergroup          0 2017-11-03 04:22 /user/reilly/tgen/_SUCCESS
-rw-r--r--   3 reilly supergroup  546133400 2017-11-03 04:22 /user/reilly/tgen/part-m-00000
-rw-r--r--   3 reilly supergroup  546133300 2017-11-03 04:22 /user/reilly/tgen/part-m-00001
-rw-r--r--   3 reilly supergroup  546133300 2017-11-03 04:22 /user/reilly/tgen/part-m-00002
-rw-r--r--   3 reilly supergroup  546133400 2017-11-03 04:21 /user/reilly/tgen/part-m-00003
-rw-r--r--   3 reilly supergroup  546133300 2017-11-03 04:21 /user/reilly/tgen/part-m-00004
-rw-r--r--   3 reilly supergroup  546133300 2017-11-03 04:22 /user/reilly/tgen/part-m-00005
-rw-r--r--   3 reilly supergroup  546133400 2017-11-03 04:21 /user/reilly/tgen/part-m-00006
-rw-r--r--   3 reilly supergroup  546133300 2017-11-03 04:21 /user/reilly/tgen/part-m-00007
-rw-r--r--   3 reilly supergroup  546133300 2017-11-03 04:22 /user/reilly/tgen/part-m-00008
-rw-r--r--   3 reilly supergroup  546133400 2017-11-03 04:22 /user/reilly/tgen/part-m-00009
-rw-r--r--   3 reilly supergroup  546133300 2017-11-03 04:22 /user/reilly/tgen/part-m-00010
-rw-r--r--   3 reilly supergroup  546133300 2017-11-03 04:22 /user/reilly/tgen/part-m-00011

```
* The command and output of  hadoop fsck -blocks /user/reilly/tgen   
```
[reilly@ip-172-31-36-244 ~]$ hadoop fsck -blocks /user/reilly/tgen
DEPRECATED: Use of this script to execute hdfs command is deprecated.
Instead use the hdfs command for it.

Connecting to namenode via http://ip-172-31-36-244.us-west-2.compute.internal:50070
FSCK started by reilly (auth:SIMPLE) from /172.31.36.244 for path /user/reilly/tgen at Fri Nov 03 04:24:26 UTC 2017
.............Status: HEALTHY
 Total size:	6553600000 B
 Total dirs:	1
 Total files:	13
 Total symlinks:		0
 Total blocks (validated):	204 (avg. block size 32125490 B)
 Minimally replicated blocks:	204 (100.0 %)
 Over-replicated blocks:	0 (0.0 %)
 Under-replicated blocks:	0 (0.0 %)
 Mis-replicated blocks:		0 (0.0 %)
 Default replication factor:	3
 Average block replication:	3.0
 Corrupt blocks:		0
 Missing replicas:		0 (0.0 %)
 Number of data-nodes:		4
 Number of racks:		1
FSCK ended at Fri Nov 03 04:24:26 UTC 2017 in 9 milliseconds


The filesystem under path '/user/reilly/tgen' is HEALTHY


```
