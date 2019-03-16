# PDFsam

In order to compile, the jdk was changed to openjdk-11 and the path is added to the pom file to use the specific java. 

* Please make change to this location based on your openjdk path. If it is already present on the system as the default java alternatives then you can replace it with the 

        <activation>
				 <jdk>(,11)</jdk>
        </activation>

- Current change for local machine at particular line number in pom.xml:

       64                         <activation>
       65                                 <jdk>/home/pkt/Downloads/jdk-11.0.2/bin/java</jdk>
       66                         </activation>

Similarly, the MakeFile also needs to be changed to include the jdk path in JAVA_HOME and update PATH to include bin folder of jdk.
