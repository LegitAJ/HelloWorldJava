java.helloworldjava
=======================

This is "Hello World" Example for Java with Maven that uses github actions
Scans are automated to run upon push to repo master branch.  edit yml file to modify. 



Compile class
-------------

To compile the main class for package, execute the follow command: ::

  mvn clean package


Run the JAR file
--------------
mvn exec:java


Isssues
--------
This scan is supposed to call AST action with SCARESOLVER option but the sca scan fails.
It appears no command line parameters can be passed to scaresolver option
The logs indicate a problem with scaresolver finding maven even though it is available in the rest of the workflow.
Program "Resolved 0 dependencies for file pom.xml. [Status=MavenNotAvailable]" 
