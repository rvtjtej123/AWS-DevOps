**Maven Commands**
***************************************

| Command | Purpose | What it does |
|---|---|---|
|mvn clean| Deletes the target directory, removing all files from previous builds to ensure a fresh start.     |      <ul><li> Cleans the Target Folder  </ul></li>|
|mvn validate  | Checks if project structure and pom.xml are correct. Checks if the project structure is correct and all dependencies are downloaded. |
|mvn compile | Compiles the source code (src/main/java) into bytecode (target/classes).     | <ul><li>Downloads&nbsp;dependencies</li><li>Compiles src/main/java</li><li>Compile Project</li></ul> |

----------------------------------------------------------------------------------------------------------------------------------------------------

* Run Tests :
    mvn test : Runs unit tests using frameworks like JUnit or TestNG. 
        What it does:
          * Compiles test classes. 
          * Runs unit tests from src/test/java

----------------------------------------------------------------------------------------------------------------------------------------------------

* Package Application :
     mvn package : Takes the compiled code and bundles it into its distributable format, such as a JAR or WAR file. 
        What it does:
          * Compiles
          * Runs tests
          * Creates: .jar or .war
          * Example output: target/myapp-1.0.jar

----------------------------------------------------------------------------------------------------------------------------------------------------

* Verify :
    mvn verify : Runs integration tests to verify the quality of the package.

----------------------------------------------------------------------------------------------------------------------------------------------------

* Install to Local Repository :
    mvn install : Installs the package into your Local Repository (~/.m2), making it available for other projects on your machine to use as a dependency.
      What it does:
          * Performs package phase
          * Copies artifact into local Maven repo
          * Located at : ~/.m2/repository

----------------------------------------------------------------------------------------------------------------------------------------------------

* Deploy to Remote Repository
    mvn deploy : Copies the final package to a Remote Repository (like Nexus or Artifactory) for sharing with other developers.
      Used in:
          * CI/CD pipelines
          * Nexus
          * Artifactory
          * Uploads build artifact to remote repository.

----------------------------------------------------------------------------------------------------------------------------------------------------
****************************************************************************************************************************************************

              * EXTRA *
***************************************
* Full Clean Build :
    mvn clean install : Most common real-world command.
      What it does:
        * Deletes old build
        * Compiles project
        * Runs tests
        * Packages artifact
        * Installs into local repo

----------------------------------------------------------------------------------------------------------------------------------------------------
