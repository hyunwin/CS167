# Lab 1

## Student information
* Full name: Hyun Bin Won
* E-mail: hwon002@ucr.edu
* UCR NetID: hwon002
* Student ID: 862098834

## Answers

* (Q1) What is the name of the created directory?
hwon002_lab1

* (Q2) What do you see at the console output?
Hello World!

* (Q3) What do you see at the output?
   log4j:WARN No appenders could be found for logger (org.apache.hadoop.metrics2.lib.MutableMetricsFactory).
   log4j:WARN Please initialize the log4j system properly.
   log4j:WARN See http://logging.apache.org/log4j/1.2/faq.html#noconfig for more info.
   WARNING: An illegal reflective access operation has occurred
   WARNING: Illegal reflective access by org.apache.hadoop.security.authentication.util.KerberosUtil (file:/C:/Users/Hyun/.m2/repository/org/apache/hadoop/hadoop-auth/2.10.0/hadoop-auth-2.10.0.jar) to method sun.security.krb5.Config.getInstance()
   WARNING: Please consider reporting this to the maintainers of org.apache.hadoop.security.authentication.util.KerberosUtil
   WARNING: Use --illegal-access=warn to enable warnings of further illegal reflective access operations
   WARNING: All illegal access operations will be denied in a future release
   
   Process finished with exit code 0
   
* (Q4) What is the output that you see at the console?
Output for file 'part-r-00000'
but	1
cannot	3
crawl	1
do	1
fly,	1
forward	1
have	1
if	3
keep	1
moving	1
run	1
run,	1
then	3
to	1
walk	1
walk,	1
whatever	1
you	5

Output:
log4j:WARN No appenders could be found for logger (org.apache.hadoop.metrics2.lib.MutableMetricsFactory).
log4j:WARN Please initialize the log4j system properly.
log4j:WARN See http://logging.apache.org/log4j/1.2/faq.html#noconfig for more info.
WARNING: An illegal reflective access operation has occurred
WARNING: Illegal reflective access by org.apache.hadoop.security.authentication.util.KerberosUtil (file:/C:/Users/Hyun/.m2/repository/org/apache/hadoop/hadoop-auth/2.10.0/hadoop-auth-2.10.0.jar) to method sun.security.krb5.Config.getInstance()
WARNING: Please consider reporting this to the maintainers of org.apache.hadoop.security.authentication.util.KerberosUtil
WARNING: Use --illegal-access=warn to enable warnings of further illegal reflective access operations
WARNING: All illegal access operations will be denied in a future release

Process finished with exit code 0

* (Q5) Does it run? Why or why not?
It does not run because the two outputs in the console depends whether the output.txt folder exists or not.
Output.txt folder exists:
log4j:WARN No appenders could be found for logger (org.apache.hadoop.metrics2.lib.MutableMetricsFactory).
log4j:WARN Please initialize the log4j system properly.
log4j:WARN See http://logging.apache.org/log4j/1.2/faq.html#noconfig for more info.
WARNING: An illegal reflective access operation has occurred
WARNING: Illegal reflective access by org.apache.hadoop.security.authentication.util.KerberosUtil (file:/C:/Users/Hyun/.m2/repository/org/apache/hadoop/hadoop-auth/2.10.0/hadoop-auth-2.10.0.jar) to method sun.security.krb5.Config.getInstance()
WARNING: Please consider reporting this to the maintainers of org.apache.hadoop.security.authentication.util.KerberosUtil
WARNING: Use --illegal-access=warn to enable warnings of further illegal reflective access operations
WARNING: All illegal access operations will be denied in a future release
Exception in thread "main" org.apache.hadoop.mapred.FileAlreadyExistsException: Output directory file:/C:/Users/Hyun/Workspace/hwon002_lab1
	at org.apache.hadoop.mapreduce.lib.output.FileOutputFormat.checkOutputSpecs(FileOutputFormat.java:146)
	at org.apache.hadoop.mapreduce.JobSubmitter.checkSpecs(JobSubmitter.java:279)
	at org.apache.hadoop.mapreduce.JobSubmitter.submitJobInternal(JobSubmitter.java:145)
	at org.apache.hadoop.mapreduce.Job$11.run(Job.java:1570)
	at org.apache.hadoop.mapreduce.Job$11.run(Job.java:1567)
	at java.base/java.security.AccessController.doPrivileged(Native Method)
	at java.base/javax.security.auth.Subject.doAs(Subject.java:423)
	at org.apache.hadoop.security.UserGroupInformation.doAs(UserGroupInformation.java:1893)
	at org.apache.hadoop.mapreduce.Job.submit(Job.java:1567)
	at org.apache.hadoop.mapreduce.Job.waitForCompletion(Job.java:1588)
	at edu.ucr.cs.cs167.hwon002.App.main(App.java:70)

Output.txt folder does not exist:
    log4j:WARN No appenders could be found for logger (org.apache.hadoop.metrics2.lib.MutableMetricsFactory).
    log4j:WARN Please initialize the log4j system properly.
    log4j:WARN See http://logging.apache.org/log4j/1.2/faq.html#noconfig for more info.
    WARNING: An illegal reflective access operation has occurred
    WARNING: Illegal reflective access by org.apache.hadoop.security.authentication.util.KerberosUtil (file:/C:/Users/campo/.m2/repository/org/apache/hadoop/hadoop-auth/2.10.0/hadoop-auth-2.10.0.jar) to method sun.security.krb5.Config.getInstance()
    WARNING: Please consider reporting this to the maintainers of org.apache.hadoop.security.authentication.util.KerberosUtil
    WARNING: Use --illegal-access=warn to enable warnings of further illegal reflective access operations
    WARNING: All illegal access operations will be denied in a future release
    
    Process finished with exit code 0
