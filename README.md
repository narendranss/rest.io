REST.IO
=======
REST.IO is a sleek and beautiful RESTful web services testing client. 
There are some testing tools already available in the market. But still we wanted to build this for showing the love towards JAX-RS specification and RESTful world.


Pre-Requisites
==============
1. Any IDE - Eclipse, Netbeans, ItelliJ for ease development.
2. Maven 3+
3. Gradle 2.1+

Steps to build Project
======================

Step 1: Import the project
==========================
Import the project as maven project in the IDE or run following commands and import them as normal project
1. For deleting - .classpath and .project files
mvn eclipse:clean 
2. For creating - .classpath and .project files
mvn eclipse:eclipse

Step 2: Build & Run Project with Maven and embedded Tomcat7 plugin
==================================================================
Either use IDE maven tools to build or cmd commands.

cmd Command to build
mvn -Dmaven.test.skip=true clean install tomcat7:run

Step 2 (alternate): Build & Run Project with Gradle
===================================================
Either use IDE maven tools to build or cmd commands.

cmd Command to build war, the generated war will be available in build/lib folder
gradle assemble

Deploy the war manually in External Server for gradle build as of now.
