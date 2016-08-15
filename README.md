# Flume

#Problem Statement:
This exercise copy local file content to HDFS using flume. 

#Requirement:
1.  Version: Flume 1.6.0-cdh5.7.0
2.  O.S.: Centos (Cloudera Virtual machine)

#Steps to run this exercise :
1.	There are 2 configuration files(avro.conf, avro2.conf ) attached in which you need to update respective files contents that is in "avro.conf" file you need to specify local file that you want to copy, and in "avro2.conf" file you need to update HDFS directory.

2.	Run following command in terminal: 
flume-ng agent -f avro2.conf -n a1.

3.	Open another terminal and run following command:
flume-ng agent --conf conf --conf-file avro.conf --name a1 Dflume.root.logger=INFO,console

4. Verify respective haddop directoy whether local file copy or not.
