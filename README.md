# SpringBootBatch
Spring Boot Batch application that take two input parameters, the first one is path to a text file, the second one is number of threads. The file content is split by line and a Caesar cipher run for each line, the final output is a encrypted text file. It uses a scheduled cron to kick of every minute and will not kick of at startup.

File input set to \resources\input\inputData2.txt with threadCount of 6.
File output is output\encodedOutputData.txt

a Jar file was created and can be found under batchdemo\target\batchdemo-0.0.1-SNAPSHOT.jar. It was created with Maven.

The batch job is not set to execute immediately, but on the minute every minute.
Exeucte the jar by running java -jar target/batchdemo-0.0.1-SNAPSHOT.jar
