Optane + CAS Test Plan
==============

Compare CAS+ Optane with HDFS Lazy Persist
-----------------

### 1. Purpose
•	Verify that Optane + CAS can be used in HDFS Low Latency Write
•	Compare the performance of Optane + CAS with RAMDISK
•	Test the HDFS writing performance

### 2. Test Environment
* Cluster： 1 Namenode + 2 Datanodes
* Disk： 5 HDDs on each datanode
* Memory : 375 GB
* Optane : 375 GB
* Hadoop version: trunk (3.0.0-beta1-SNAPSHOT)

### 3.WorkLoad
•	Use TestDFSIO tool to measure the performance. 
•	1 replica
•	Test cases:

| Case Name | Storage | Dataset | Comment |
| --------- | ------- | ------- | ------- |
| 100G_RAM_HDD | 1Optane 5HDDs | 100G | Using HDFS lazy persist mode |

### 4. Performance Measurement
Throughput of the writing

 
 

