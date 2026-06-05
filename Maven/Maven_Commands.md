<h1 align="center"> * Maven Commands *</h1>

| Command | Purpose | What it does |
|---|---|---|
|`mvn clean`| Deletes the target directory, removing all files from previous builds to ensure a fresh start.     |      <ul><li> Cleans the Target Folder  </ul></li>|
|`mvn validate`  | Checks if project structure and pom.xml are correct. Checks if the project structure is correct and all dependencies are downloaded. |
|`mvn compile` | Compiles the source code (src/main/java) into bytecode (target/classes).     | <ul><li>Downloads&nbsp;dependencies</li><li>Compiles src/main/java</li><li>Compile Project</li></ul> |
| `mvn test` | Runs unit tests using frameworks like JUnit or TestNG. | <ul><li>Compiles test classes</li><li>Runs unit tests from src/test/java</li></ul>|
| `mvn package` | Takes the compiled code and bundles it into its distributable format, such as a JAR or WAR file. | <ul><li>Package Application</li> <li> Compiles </li> <li>Runs tests </li> <li> Creates: .jar or .war</li> <li>Example output: target/myapp-1.0.jar </li> </ul> |
| `mvn verify` | Runs integration tests to verify the quality of the package. |
|  `mvn install` | Installs the package into your Local Repository (~/.m2), making it available for other projects on your machine to use as a dependency. | <ul><li> Install to Local Repository. <li>Performs package phase</li> <li> Copies artifact into local Maven repo </li>  <li> Located at : ~/.m2/repository</li> </ul>
| `mvn deploy` | Copies the final package to a Remote Repository (like Nexus or Artifactory) for sharing with other developers. | <ul><li>Deploy to Remote Repository</li> ✤ **NOTE** : **USED IN** ✤ <li>CI/CD pipelines</li> <li>Nexus</li>  <li>Artifactory</li> <li>Uploads build artifact to remote repository.</li> </ul>


----------------------------------------------------------------------------------------------------------------------------------------------------
****************************************************************************************************************************************************

   <h1 align="center"> * Extra *</h1>   
   
| Command | Purpose | What it does |
|---|---|---|
`mvn clean install` | Most common real-world command. | <ul><li>Full Clean Build</li> <li>Deletes old build</li>  <li>Compiles project </li>  <li>Runs tests </li> <li>Packages artifact <li>Installs into local repo </li></ul>
   
