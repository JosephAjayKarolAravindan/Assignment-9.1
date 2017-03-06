Session 9: Assignment 1

1.	Why MapReduce program is needed in Pig Programming

 In MapReduce mode, Pig translates queries into MapReduce jobs and runs them on a Hadoop cluster. The cluster may be a pseudo- or fully distributed cluster. MapReduce mode is used to run Pig on large datasets.

2.	What are advantages of pig over MapReduce

•	Pig is a scripting language 
•	Higher level of abstraction 
•	Comparatively less lines compared to MapReduce
•	Development effort is less


3.	What is pig engine and what is its importance

Apache Pig has a component known as Pig Engine that accepts the Pig Latin scripts as input and converts those scripts into MapReduce jobs.
Importance of pig engine is that it acts as an interpreter between pig latin script and MapReduce jobs. It creates environment to execute Pig scripts into series of MapReduce jobs in parallel manner.

4.	What are the modes of Pig execution

Pig has two execution modes or types. They are:

Local Mode
MapReduce Mode



Local Mode: 
In Local Mode of Pig execution, all the input data will be taken from local file system. After execution it provides output on top of local file system.  In local mode, Pig runs in a single JVM and accesses the local filesystem. This mode of suitable only for small datasets and when trying out Pig. To start the local mode of execution, the following command is used.   
•	# pig -x local

The above command starts Grunt. Grunt is the Pig interactive shell. 

MapReduce Mode/HDFS Mode/ Clustered Mode: 

In this mode Apache Pig will take the input form HDFS paths only, and after processing data it will put output files on top of HDFS. In MapReduce mode of execution, Pig translates queries into MapReduce jobs and runs them on a Hadoop Cluster.  

5.	What is grunt shell in Pig

The Grunt shell can run Pig scripts in the shell. The Grunt shell of Apache Pig is mainly used to write Pig Latin scripts.

6.	What are the features of Pig Latin language

•	Loading and storing of data
•	Streaming data
•	Filtering data
•	Grouping and joining data
•	Sorting data
•	Combining and splitting data

7.	Is Pig latin commands case sensitive

The names (aliases) of relations and fields are case sensitive. The names of Pig Latin functions are case sensitive. The names of parameters (see Parameter Substitution) and all other Pig Latin keywords are case insensitive.
In the example below, note the following:
•	The names (aliases) of relations A, B, and C are case sensitive.
•	The names (aliases) of fields f1, f2, and f3 are case sensitive.
•	Function names PigStorage and COUNT are case sensitive.
•	Keywords LOAD, USING, AS, GROUP, BY, FOREACH, GENERATE, and DUMP are case insensitive. They can also be written as load, using, as, group, by, etc.
•	In the FOREACH statement, the field in relation B is referred to by positional notation.


8.	What is a data flow language

Dataflow programming is a programming paradigm that models a program as a directed graph of the data flowing between operations, thus implementing dataflow principles and architecture. Dataflow programming languages share some features of functional languages, and were generally developed in order to bring some functional concepts to a language more suitable for numeric processing.



