## MapReduce

We need to create a gradle project and then implement the logic in the WordCount.java which is our mainClassName. Then, we need to follow a few steps to make sure the build.gradle is configured correctly and a few more touch points. 

Below are the required steps:

1. Add artifacts to the Project Structure. In IntelliJ, File->Project Structure->Artifacts->Click on the + icon. 
2. Make sure the build.gradle has all the important commands such as all the dependencies, and jar configuration includes dependencies as well. 
3. Then, clean and build the project. In IntelliJ, these options are available on the right side of the ide. After building the project successfully, the jar file can be found in project directory->build->libs. 
4. Upload the jar file to the server. We can run the jar file before uploading by running this command: java -jar <file-name.jar>
5. Finally, make sure the input file is present on the hdfs and then run this command: hadoop jar <file-name.jar> inputfile outputfile. Ex: hadoop jar mapreduce-1.0-SNAPSHOT.jar ./test.txt output1
