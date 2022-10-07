Video URL : https://drive.google.com/file/d/1SNkMzmiJKqGH8YIwW8aOFlMU1-HMmRfI/view?usp=sharing



## Build Process in java based project/application management:

Developers duty/responsibility to develop a java based business application:

1.Write source code(bunch of classes, inteface...) 

2.add some external  jarfiles to the classpath (dependencies of our application)
in JDBC dao project, driver jar file is the dependency of our project.

3.compile the code.

4.prepare some test cases (Unit test) 

5.add Junit/mockito related jar files inside the classpath

6.compile and run the test cases.

7.arrange our code in a standard folder structure

Java based Webapplication:

.java

.class

.jar

.html

.css

.js

.xml files

.mp3, mp4, jpg, gif 

8.Do the packaging : build the jar, war file. 

9.deploy this jar file/ war file to the server.


If any mistake identified then developer performs above task again and again.

To automate this build process of java applicaiton, Apache foundation released build tool called Maven.

## What is Build Tool?

Build tools are programs that automate the creation of executable applications from
source code (e.g., .apk for an Android app).

Example of Build tool - Ant,Maven,Gradle.

## Maven

Maven is a tool that can now be used for building and managing any Java-based project. It makes the day-to-day
work of Java developers easier and generally help with the comprehension of any Java-based project.
Maven is a powerful project management tool that is based on POM (project object model). It is used for projects
build, dependency and documentation.

Dependency is defined as a state of needing something or someone.
When you rely on coffee to get you through the day, this is an example of you having dependency on caffeine
(coffee).
In Maven, a dependency is just another archive—JAR, ZIP, and so on—which our current project needs in order
to compile, build, test, and/or run. These project dependencies are collectively specified in the pom. xml file,
inside of a <dependencies> tag.


## Maven Build Life cycle:
  
  1.validate: - in this phase it will verify the project diectory structure is valid or not. and it has pom.xml file is there or not.

  2.compile: maven compiles all the source code of the project by downloading and adding requied jar files in the classpath.

  3.test-compile: if we have written any unit test cases those code will be compiled.

  4.test : maven will run all the test cases and it will show how many test cases are success and how many fails.

  5.package : maven will bundle our java code into a jar file inside 'target' folder.

  6.install : that jar file in step 5 will be stored in the localrepo.

  7.deploy : maven stores the application jar file to the central repo.

  8.clean : here maven will delete and remove all the files that are generated in previous build. this phase is an isolated phase.
  
  Note: if we execute any phase to build the maven project then maven will execute all the phases till that given phase.except phase 8.clean.
 
  >mvn clean   :- remove and delete previous build
  >mvn test   : till the test phase.
  >mvn deploy: 
  >mvn validate:
  
  
  We can develop java application using Maven in 2 ways:
  
  1. Using console based
  2. Using IDE
  
  ## Maven terminology:

  1. Artifact (project) :

    An artifact is an outcome in maven, it can be a file, .class file or a jar file, war file,ear file,etc.

  2. Archetype :

    It is project template for creating similar type of project in maven.

  3. Groupid : 

    It is an Id used to identify the artifacts of a perticular organization (naming convention is similar to package name.) com.wipro
  
  4. Artifactid : 
    
    It is the id for the final outcome (artifactid name will be the root folder of our application)

  5. pom.xml (project object model) :
    
    All the information will be their in this file. In this model, entire application itself will be considered as an object.

    It defines following properties for a project:

    1. Name

    2.version

    3. packaging (jar, war, ear)

    4.dependecnies : required jar files.

    5.plugins: will inhance the functionality of our project.

    docker

    jenkins (CI/CD)
  
  ## Maven Repository :
  
  A repository is a store where maven maintains plugins, archetypes, and lots of jar files used for building different kinds of java projects.

  Maven repository are of 3 types:
  
  1.central repo : it is the maven's own repo in which it maintains all kinds of project related plugins, archetypes, jars etc.

  https://repo1.maven.org/maven2

  2.remote repo : this repo is maintained within the organization for sharing plugins, archetypes and jar files for multiple projects withing orgnizations. ex: masairepo

  3.local repo : this repo will be created inside the developer computer.  (.m2) is the name for this repo.

  mysql-connector.jar 

  pom.xml

  package.json

  .m2 
  
  
  
