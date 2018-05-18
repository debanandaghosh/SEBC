[hdfs@instance-2 ~]$ time yarn jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar teragen -Dmapred.map.tasks=40 -Ddfs.block.size=67108864 5242880 /use
r/groot/tgen
18/05/18 05:27:22 INFO Configuration.deprecation: session.id is deprecated. Instead, use dfs.metrics.session-id
18/05/18 05:27:22 INFO jvm.JvmMetrics: Initializing JVM Metrics with processName=JobTracker, sessionId=
18/05/18 05:27:23 INFO terasort.TeraGen: Generating 5242880 using 1
18/05/18 05:27:23 INFO mapreduce.JobSubmitter: number of splits:1
18/05/18 05:27:23 INFO Configuration.deprecation: dfs.block.size is deprecated. Instead, use dfs.blocksize
18/05/18 05:27:23 INFO Configuration.deprecation: mapred.map.tasks is deprecated. Instead, use mapreduce.job.maps
18/05/18 05:27:23 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_local164074215_0001
18/05/18 05:27:23 INFO mapreduce.Job: The url to track the job: http://localhost:8080/
18/05/18 05:27:23 INFO mapreduce.Job: Running job: job_local164074215_0001
18/05/18 05:27:23 INFO mapred.LocalJobRunner: OutputCommitter set in config null
18/05/18 05:27:23 INFO output.FileOutputCommitter: File Output Committer Algorithm version is 1
18/05/18 05:27:23 INFO mapred.LocalJobRunner: OutputCommitter is org.apache.hadoop.mapreduce.lib.output.FileOutputCommitter
18/05/18 05:27:23 INFO mapred.LocalJobRunner: Waiting for map tasks
18/05/18 05:27:23 INFO mapred.LocalJobRunner: Starting task: attempt_local164074215_0001_m_000000_0
18/05/18 05:27:23 INFO output.FileOutputCommitter: File Output Committer Algorithm version is 1
18/05/18 05:27:23 INFO mapred.Task:  Using ResourceCalculatorProcessTree : [ ]
18/05/18 05:27:23 INFO mapred.MapTask: Processing split: org.apache.hadoop.examples.terasort.TeraGen$RangeInputFormat$RangeInputSplit@4783eac4
18/05/18 05:27:24 INFO mapreduce.Job: Job job_local164074215_0001 running in uber mode : false
18/05/18 05:27:24 INFO mapreduce.Job:  map 0% reduce 0%
18/05/18 05:27:35 INFO mapred.LocalJobRunner: map > map
18/05/18 05:27:36 INFO mapreduce.Job:  map 8% reduce 0%
18/05/18 05:27:41 INFO mapred.LocalJobRunner: map > map
18/05/18 05:27:42 INFO mapreduce.Job:  map 12% reduce 0%
18/05/18 05:27:47 INFO mapred.LocalJobRunner: map > map
18/05/18 05:27:48 INFO mapreduce.Job:  map 15% reduce 0%
18/05/18 05:27:53 INFO mapred.LocalJobRunner: map > map
18/05/18 05:27:54 INFO mapreduce.Job:  map 19% reduce 0%
18/05/18 05:27:59 INFO mapred.LocalJobRunner: map > map
18/05/18 05:28:00 INFO mapreduce.Job:  map 23% reduce 0%
18/05/18 05:28:05 INFO mapred.LocalJobRunner: map > map
18/05/18 05:28:06 INFO mapreduce.Job:  map 26% reduce 0%
18/05/18 05:28:11 INFO mapred.LocalJobRunner: map > map
18/05/18 05:28:12 INFO mapreduce.Job:  map 30% reduce 0%
18/05/18 05:28:17 INFO mapred.LocalJobRunner: map > map
18/05/18 05:28:18 INFO mapreduce.Job:  map 34% reduce 0%
18/05/18 05:28:23 INFO mapred.LocalJobRunner: map > map
18/05/18 05:28:24 INFO mapreduce.Job:  map 38% reduce 0%
18/05/18 05:28:29 INFO mapred.LocalJobRunner: map > map
18/05/18 05:28:30 INFO mapreduce.Job:  map 41% reduce 0%
18/05/18 05:28:35 INFO mapred.LocalJobRunner: map > map
18/05/18 05:28:36 INFO mapreduce.Job:  map 45% reduce 0%
18/05/18 05:28:41 INFO mapred.LocalJobRunner: map > map
18/05/18 05:28:42 INFO mapreduce.Job:  map 49% reduce 0%
18/05/18 05:28:47 INFO mapred.LocalJobRunner: map > map
18/05/18 05:28:48 INFO mapreduce.Job:  map 52% reduce 0%
18/05/18 05:28:53 INFO mapred.LocalJobRunner: map > map
18/05/18 05:28:54 INFO mapreduce.Job:  map 54% reduce 0%
18/05/18 05:28:59 INFO mapred.LocalJobRunner: map > map
18/05/18 05:29:00 INFO mapreduce.Job:  map 57% reduce 0%
18/05/18 05:29:05 INFO mapred.LocalJobRunner: map > map
18/05/18 05:29:06 INFO mapreduce.Job:  map 59% reduce 0%
18/05/18 05:29:11 INFO mapred.LocalJobRunner: map > map
18/05/18 05:29:12 INFO mapreduce.Job:  map 61% reduce 0%
18/05/18 05:29:17 INFO mapred.LocalJobRunner: map > map
18/05/18 05:29:18 INFO mapreduce.Job:  map 63% reduce 0%
18/05/18 05:29:23 INFO mapred.LocalJobRunner: map > map
18/05/18 05:29:24 INFO mapreduce.Job:  map 65% reduce 0%
18/05/18 05:29:29 INFO mapred.LocalJobRunner: map > map
18/05/18 05:29:30 INFO mapreduce.Job:  map 69% reduce 0%
18/05/18 05:29:35 INFO mapred.LocalJobRunner: map > map
18/05/18 05:29:36 INFO mapreduce.Job:  map 73% reduce 0%
18/05/18 05:29:41 INFO mapred.LocalJobRunner: map > map
18/05/18 05:29:42 INFO mapreduce.Job:  map 77% reduce 0%
18/05/18 05:29:47 INFO mapred.LocalJobRunner: map > map
18/05/18 05:29:48 INFO mapreduce.Job:  map 80% reduce 0%
18/05/18 05:29:53 INFO mapred.LocalJobRunner: map > map
18/05/18 05:29:54 INFO mapreduce.Job:  map 84% reduce 0%
18/05/18 05:29:59 INFO mapred.LocalJobRunner: map > map
18/05/18 05:30:00 INFO mapreduce.Job:  map 88% reduce 0%
18/05/18 05:30:05 INFO mapred.LocalJobRunner: map > map
18/05/18 05:30:06 INFO mapreduce.Job:  map 91% reduce 0%
18/05/18 05:30:11 INFO mapred.LocalJobRunner: map > map
18/05/18 05:30:12 INFO mapreduce.Job:  map 93% reduce 0%
18/05/18 05:30:17 INFO mapred.LocalJobRunner: map > map
18/05/18 05:30:18 INFO mapreduce.Job:  map 95% reduce 0%
18/05/18 05:30:23 INFO mapred.LocalJobRunner: map > map
18/05/18 05:30:24 INFO mapreduce.Job:  map 97% reduce 0%
18/05/18 05:30:29 INFO mapred.LocalJobRunner: map > map
18/05/18 05:30:30 INFO mapreduce.Job:  map 99% reduce 0%
18/05/18 05:30:30 INFO mapred.LocalJobRunner: map > map
18/05/18 05:30:33 INFO mapred.Task: Task:attempt_local164074215_0001_m_000000_0 is done. And is in the process of committing
18/05/18 05:30:33 INFO mapred.LocalJobRunner: map > map
18/05/18 05:30:33 INFO mapred.Task: Task attempt_local164074215_0001_m_000000_0 is allowed to commit now
18/05/18 05:30:33 INFO output.FileOutputCommitter: Saved output of task 'attempt_local164074215_0001_m_000000_0' to hdfs://instance-1.c.golden-veld-204308.internal:8020/user/g
root/tgen/_temporary/0/task_local164074215_0001_m_000000
18/05/18 05:30:33 INFO mapred.LocalJobRunner: map
18/05/18 05:30:33 INFO mapred.Task: Task 'attempt_local164074215_0001_m_000000_0' done.
18/05/18 05:30:33 INFO mapred.LocalJobRunner: Finishing task: attempt_local164074215_0001_m_000000_0
18/05/18 05:30:33 INFO mapred.LocalJobRunner: map task executor complete.
18/05/18 05:30:34 INFO mapreduce.Job:  map 100% reduce 0%
18/05/18 05:30:34 INFO mapreduce.Job: Job job_local164074215_0001 completed successfully
18/05/18 05:30:34 INFO mapreduce.Job: Counters: 21
        File System Counters
                FILE: Number of bytes read=276515
                FILE: Number of bytes written=574670
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=0
                HDFS: Number of bytes written=524288000
                HDFS: Number of read operations=4
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=3
        Map-Reduce Framework
                Map input records=5242880
                Map output records=5242880
                Input split bytes=82
                Spilled Records=0
                Failed Shuffles=0
                Merged Map outputs=0
                GC time elapsed (ms)=43
                Total committed heap usage (bytes)=370671616
        org.apache.hadoop.examples.terasort.TeraGen$Counters
                CHECKSUM=11257830824958050
        File Input Format Counters 
                Bytes Read=0
        File Output Format Counters 
                Bytes Written=524288000
real    3m13.401s
user    0m15.176s
sys     0m1.386s



[hdfs@instance-2 ~]$ hdfs dfs -ls /user/groot/tgen
Found 2 items
-rw-r--r--   3 hdfs supergroup          0 2018-05-18 05:30 /user/groot/tgen/_SUCCESS
-rw-r--r--   3 hdfs supergroup  524288000 2018-05-18 05:30 /user/groot/tgen/part-m-00000
[hdfs@instance-2 ~]$ hadoop fsck -blocks /user/groot
DEPRECATED: Use of this script to execute hdfs command is deprecated.
Instead use the hdfs command for it.
Connecting to namenode via http://instance-1.c.golden-veld-204308.internal:50070
FSCK started by hdfs (auth:SIMPLE) from /10.142.0.3 for path /user/groot at Fri May 18 05:31:29 UTC 2018
..Status: HEALTHY
 Total size:    524288000 B
 Total dirs:    2
 Total files:   2
 Total symlinks:                0
 Total blocks (validated):      8 (avg. block size 65536000 B)
 Minimally replicated blocks:   8 (100.0 %)
 Over-replicated blocks:        0 (0.0 %)
 Under-replicated blocks:       0 (0.0 %)
 Mis-replicated blocks:         0 (0.0 %)
 Default replication factor:    3
 Average block replication:     3.0
 Corrupt blocks:                0
 Missing replicas:              0 (0.0 %)
 Number of data-nodes:          3
 Number of racks:               1
FSCK ended at Fri May 18 05:31:29 UTC 2018 in 2 milliseconds
