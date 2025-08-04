# Maven

## About:
Maven is a build and configuration tool for Java.


1. to validate is maven is available:
```bash
mvn --version
```

2. to generate a configuration using maven:
```bash
mvn archetype:generate
```
  - now the thing is above command will share all templates that are uploaded to maven repository
  - so below command is filter to select only official maven templates
```
mvn archetype:generate "-Dfilter=org.apache.maven.archetypes:"
```

important fields while creating project:
- groupId
    - used for creating unique folder for the project
    - e.g., com.apache.maven
- artifactId
    - used for creating the unique .war or .jar file-name
    - e.g., maven-crash will lead to having maven-crash.jar file created for deployment.
- version
    - for version number for the .war or .jar creation.
    - e.g., 1.0 will lead to having mave-crash-1.0.jar will be created for deployment.
- package
    - for creating the directory where all the java files will be placed as single package.
    - also groupID and package are kept same for simlicity as standards.
    - e.g., com.apache.maven will lead to creation of com/apache/maven/ package directory wherein all .java files will reside.
*the first 3 values are also referred to as GAV or Maven GAV *