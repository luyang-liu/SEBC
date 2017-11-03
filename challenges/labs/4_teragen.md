* The full  teragen  command and output
```
time hadoop jar /opt/cloudera/parcels/CDH/jars/hadoop*-examples.jar teragen -Dmapred.map.tasks=8 -Ddfs.block.size=67108864 -Dyarn.nodemanager.resource.memory-mb=536870912 65536000  /user/jimenez/tgen
```
@mfernest: the property `Dyarn.nodemanager.resource.memory-mb` does not set a container size for a task. It could set the resource limit on a NodeManager, but in this case the value is too large and would be ignored.
```
17/10/13 03:46:09 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-40-116.us-west-2.compute.internal/172.31.40.116:8032
17/10/13 03:46:10 INFO terasort.TeraSort: Generating 65536000 using 8
17/10/13 03:46:11 INFO mapreduce.JobSubmitter: number of splits:8
17/10/13 03:46:11 INFO Configuration.deprecation: mapred.map.tasks is deprecated. Instead, use mapreduce.job.maps
17/10/13 03:46:11 INFO Configuration.deprecation: dfs.block.size is deprecated. Instead, use dfs.blocksize
17/10/13 03:46:11 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1507863049566_0003
17/10/13 03:46:11 INFO impl.YarnClientImpl: Submitted application application_1507863049566_0003
17/10/13 03:46:12 INFO mapreduce.Job: The url to track the job: http://ip-172-31-40-116.us-west-2.compute.internal:8088/proxy/application_1507863049566_0003/
17/10/13 03:46:12 INFO mapreduce.Job: Running job: job_1507863049566_0003
17/10/13 03:46:24 INFO mapreduce.Job: Job job_1507863049566_0003 running in uber mode : false
17/10/13 03:46:24 INFO mapreduce.Job:  map 0% reduce 0%
17/10/13 03:46:36 INFO mapreduce.Job:  map 7% reduce 0%
17/10/13 03:46:39 INFO mapreduce.Job:  map 10% reduce 0%
17/10/13 03:46:42 INFO mapreduce.Job:  map 12% reduce 0%
17/10/13 03:46:45 INFO mapreduce.Job:  map 15% reduce 0%
17/10/13 03:46:48 INFO mapreduce.Job:  map 17% reduce 0%
17/10/13 03:46:51 INFO mapreduce.Job:  map 19% reduce 0%
17/10/13 03:46:54 INFO mapreduce.Job:  map 22% reduce 0%
17/10/13 03:46:57 INFO mapreduce.Job:  map 24% reduce 0%
17/10/13 03:46:58 INFO mapreduce.Job:  map 25% reduce 0%
17/10/13 03:47:00 INFO mapreduce.Job:  map 26% reduce 0%
17/10/13 03:47:01 INFO mapreduce.Job:  map 29% reduce 0%
17/10/13 03:47:03 INFO mapreduce.Job:  map 30% reduce 0%
17/10/13 03:47:04 INFO mapreduce.Job:  map 32% reduce 0%
17/10/13 03:47:07 INFO mapreduce.Job:  map 34% reduce 0%
17/10/13 03:47:09 INFO mapreduce.Job:  map 37% reduce 0%
17/10/13 03:47:11 INFO mapreduce.Job:  map 38% reduce 0%
17/10/13 03:47:21 INFO mapreduce.Job:  map 42% reduce 0%
17/10/13 03:47:24 INFO mapreduce.Job:  map 45% reduce 0%
17/10/13 03:47:27 INFO mapreduce.Job:  map 47% reduce 0%
17/10/13 03:47:30 INFO mapreduce.Job:  map 50% reduce 0%
17/10/13 03:47:33 INFO mapreduce.Job:  map 52% reduce 0%
17/10/13 03:47:36 INFO mapreduce.Job:  map 54% reduce 0%
17/10/13 03:47:37 INFO mapreduce.Job:  map 55% reduce 0%
17/10/13 03:47:39 INFO mapreduce.Job:  map 56% reduce 0%
17/10/13 03:47:40 INFO mapreduce.Job:  map 57% reduce 0%
17/10/13 03:47:42 INFO mapreduce.Job:  map 59% reduce 0%
17/10/13 03:47:43 INFO mapreduce.Job:  map 61% reduce 0%
17/10/13 03:47:45 INFO mapreduce.Job:  map 64% reduce 0%
17/10/13 03:47:46 INFO mapreduce.Job:  map 65% reduce 0%
17/10/13 03:47:48 INFO mapreduce.Job:  map 67% reduce 0%
17/10/13 03:47:49 INFO mapreduce.Job:  map 68% reduce 0%
17/10/13 03:47:51 INFO mapreduce.Job:  map 70% reduce 0%
17/10/13 03:47:52 INFO mapreduce.Job:  map 71% reduce 0%
17/10/13 03:47:55 INFO mapreduce.Job:  map 74% reduce 0%
17/10/13 03:47:57 INFO mapreduce.Job:  map 75% reduce 0%
17/10/13 03:48:07 INFO mapreduce.Job:  map 78% reduce 0%
17/10/13 03:48:09 INFO mapreduce.Job:  map 81% reduce 0%
17/10/13 03:48:10 INFO mapreduce.Job:  map 82% reduce 0%
17/10/13 03:48:12 INFO mapreduce.Job:  map 83% reduce 0%
17/10/13 03:48:13 INFO mapreduce.Job:  map 84% reduce 0%
17/10/13 03:48:15 INFO mapreduce.Job:  map 85% reduce 0%
17/10/13 03:48:16 INFO mapreduce.Job:  map 86% reduce 0%
17/10/13 03:48:18 INFO mapreduce.Job:  map 87% reduce 0%
17/10/13 03:48:19 INFO mapreduce.Job:  map 89% reduce 0%
17/10/13 03:48:21 INFO mapreduce.Job:  map 91% reduce 0%
17/10/13 03:48:22 INFO mapreduce.Job:  map 93% reduce 0%
17/10/13 03:48:24 INFO mapreduce.Job:  map 94% reduce 0%
17/10/13 03:48:25 INFO mapreduce.Job:  map 95% reduce 0%
17/10/13 03:48:27 INFO mapreduce.Job:  map 96% reduce 0%
17/10/13 03:48:28 INFO mapreduce.Job:  map 97% reduce 0%
17/10/13 03:48:30 INFO mapreduce.Job:  map 99% reduce 0%
17/10/13 03:48:33 INFO mapreduce.Job:  map 100% reduce 0%
17/10/13 03:48:33 INFO mapreduce.Job: Job job_1507863049566_0003 completed successfully
17/10/13 03:48:33 INFO mapreduce.Job: Counters: 31
	File System Counters
		FILE: Number of bytes read=0
		FILE: Number of bytes written=979608
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=682
		HDFS: Number of bytes written=6553600000
		HDFS: Number of read operations=32
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=16
	Job Counters 
		Launched map tasks=8
		Other local map tasks=8
		Total time spent by all maps in occupied slots (ms)=335842
		Total time spent by all reduces in occupied slots (ms)=0
		Total time spent by all map tasks (ms)=335842
		Total vcore-seconds taken by all map tasks=335842
		Total megabyte-seconds taken by all map tasks=343902208
	Map-Reduce Framework
		Map input records=65536000
		Map output records=65536000
		Input split bytes=682
		Spilled Records=0
		Failed Shuffles=0
		Merged Map outputs=0
		GC time elapsed (ms)=1454
		CPU time spent (ms)=137390
		Physical memory (bytes) snapshot=2957119488
		Virtual memory (bytes) snapshot=12479295488
		Total committed heap usage (bytes)=2210922496
	org.apache.hadoop.examples.terasort.TeraGen$Counters
		CHECKSUM=140750829423462787
	File Input Format Counters 
		Bytes Read=0
	File Output Format Counters 
		Bytes Written=6553600000

real	2m27.871s
user	0m6.761s
sys	0m0.819s

```
* The result of the  time  command
```
real	2m27.871s
user	0m6.761s
sys	0m0.819s
```
* The command and output of  hdfs dfs -ls /user/jimenez/tgen 
```
hdfs dfs -ls /user/jimenez/tgen
Found 9 items
-rw-r--r--   3 jimenez supergroup          0 2017-10-13 03:48 /user/jimenez/tgen/_SUCCESS
-rw-r--r--   3 jimenez supergroup  819200000 2017-10-13 03:47 /user/jimenez/tgen/part-m-00000
-rw-r--r--   3 jimenez supergroup  819200000 2017-10-13 03:47 /user/jimenez/tgen/part-m-00001
-rw-r--r--   3 jimenez supergroup  819200000 2017-10-13 03:47 /user/jimenez/tgen/part-m-00002
-rw-r--r--   3 jimenez supergroup  819200000 2017-10-13 03:47 /user/jimenez/tgen/part-m-00003
-rw-r--r--   3 jimenez supergroup  819200000 2017-10-13 03:47 /user/jimenez/tgen/part-m-00004
-rw-r--r--   3 jimenez supergroup  819200000 2017-10-13 03:47 /user/jimenez/tgen/part-m-00005
-rw-r--r--   3 jimenez supergroup  819200000 2017-10-13 03:48 /user/jimenez/tgen/part-m-00006
-rw-r--r--   3 jimenez supergroup  819200000 2017-10-13 03:48 /user/jimenez/tgen/part-m-00007

```
* The command and output of  hadoop fsck -blocks /user/jimenez  
```
$hadoop fsck -blocks /user/jimenez 
DEPRECATED: Use of this script to execute hdfs command is deprecated.
Instead use the hdfs command for it.

Connecting to namenode via http://ip-172-31-40-116.us-west-2.compute.internal:50070
FSCK started by jimenez (auth:SIMPLE) from /172.31.40.116 for path /user/jimenez at Fri Oct 13 03:49:29 UTC 2017
..........................Status: HEALTHY
 Total size:	19660800000 B
 Total dirs:	20
 Total files:	26
 Total symlinks:		0
 Total blocks (validated):	312 (avg. block size 63015384 B)
 Minimally replicated blocks:	312 (100.0 %)
 Over-replicated blocks:	0 (0.0 %)
 Under-replicated blocks:	0 (0.0 %)
 Mis-replicated blocks:		0 (0.0 %)
 Default replication factor:	3
 Average block replication:	3.0
 Corrupt blocks:		0
 Missing replicas:		0 (0.0 %)
 Number of data-nodes:		4
 Number of racks:		1
FSCK ended at Fri Oct 13 03:49:29 UTC 2017 in 43 milliseconds


The filesystem under path '/user/jimenez' is HEALTHY


```
