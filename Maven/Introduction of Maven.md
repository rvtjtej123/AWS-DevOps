<h1 align="center"> ☆ Introduction of Maven ☆</h1>

<h2 align="left"> ➤ Maven Build Lifecycle </h2>

&nbsp;&nbsp; ● Maven uses the **JDK (Java Development Kit)** to compile and build Java applications.

&nbsp;&nbsp; ● Maven cannot run without Java being installed.

&nbsp;&nbsp; ● If we install Maven, it automatically installs JDK.21.

&nbsp;&nbsp; ● Maven uses the JDK to compile Java applications.

&nbsp;&nbsp; ● The JDK provides the compiler required to convert Java source code into executable bytecode.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **<h3> ✦ mvn validate:</h3>** 

&nbsp;&nbsp;&nbsp;&nbsp;● Validates the project structure and configuration. 

&nbsp;&nbsp;&nbsp;&nbsp;● Checks whether the pom.xml file exists and is valid

&nbsp;&nbsp;&nbsp;&nbsp;● Verifies that all required project information is correctly configured.

&nbsp;&nbsp;&nbsp;&nbsp;● Checks the project configuration and validates the pom.xml file.

&nbsp;&nbsp;&nbsp;&nbsp;● `Short Version:` It checks the configuration. Ex.:  It checks whether pom.xml file is there or not.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **<h3> ✦ mvn compile:</h3>** 

&nbsp;&nbsp;&nbsp;&nbsp;● Compiles the source code and identifies syntax/compilation errors.


&nbsp;&nbsp;&nbsp;&nbsp;● Compile all Java source files.

&nbsp;&nbsp;&nbsp;&nbsp;● Generate .class files.

&nbsp;&nbsp;&nbsp;&nbsp;● Report syntax and compilation errors.

&nbsp;&nbsp;&nbsp;&nbsp;● Compilation is the process of converting Java source code (.java) into bytecode (.class) and checking for syntax/compilation errors.

&nbsp;&nbsp;&nbsp;&nbsp;● Compile means converting human-readable Java source code (.java) into machine-readable bytecode (.class) that the computer can

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; execute.

&nbsp;&nbsp;&nbsp;&nbsp;● `Short Version:` Compiles Java source code into .class files and checks for syntax errors.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **<h3> ✦ mvn test:</h3>** 

&nbsp;&nbsp;&nbsp;&nbsp;● Compiles the application code (if not already compiled).

&nbsp;&nbsp;&nbsp;&nbsp;● Compiles the test code.

&nbsp;&nbsp;&nbsp;&nbsp;● Runs the unit testing

&nbsp;&nbsp;&nbsp;&nbsp;● Runs Unit Tests to verify that individual components of the application work correctly.

<h1 align="center"> </h1>

<h2 align="left"> ➤ Build Tool </h2>

**<h3><br>✦ Package & Dependency Management: </br></h3>**

&nbsp;&nbsp; ● We can install, update, and remove packages/dependencies using a configuration or reference file.
  
&nbsp;&nbsp; ● Different programming languages use different build and dependency management tools:

<br> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  • If the Program/Code is written in `Java`, then we use `Maven`, `Ant`, or `Gradle`. </br>
<br> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  • If the Program/Code is written in `DotNET`, then we use `MS Build` or `Visual Studio`. </br>
<br> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  • If the Program/Code is written in `Python`, then we use `PIP`. </br>
<br> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  • If the Program/Code is written in `NodeJS`, then we use  `NPM`. </br>
<br> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  • If the Program/Code is written in `Dart`, then we use  `Flutter`. </br>

<br>
<br>

  **<h3>✦ Source Code Compilation: </h3>**  
&nbsp;&nbsp; ● Source code means the application code that we stored in GitHub.

&nbsp;&nbsp; ● During compilation, syntax errors are identified.

&nbsp;&nbsp; ● If there are syntax errors in the source code, the application may fail to build or run correctly.

&nbsp;&nbsp; ● It will also compile the source code.

<br>
<br>

  **<h3>✦ Testing: </h3>**  

&nbsp;&nbsp; ● Testing is performed to verify that the application works correctly and is free from defects.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ● **Types of Testing:** Unit Testing & Integration Testing

| Unit Testing | Integration Testing |
|---|---|
|   <ul><li> Tests a small part (unit) of the application, such as a function, method, or class. |   <ul><li> Testing the interaction between multiple components/modules of an application |
|   <ul><li> Usually performed by developers.|  <ul><li> Entire application testing.|


&nbsp;&nbsp; ● Maven can be used to run both Unit Testing and Integration Testing.

<h1 align="center"> </h1>

**<h3>✦ In Short: </h3>**  

&nbsp;&nbsp; ● mvn validate → Check configuration

&nbsp;&nbsp; ● mvn compile → Compile code

&nbsp;&nbsp; ● mvn test → Run unit tests

&nbsp;&nbsp; ● mvn package → Create JAR/WAR

&nbsp;&nbsp; ● mvn verify → Run integration checks

&nbsp;&nbsp; ● mvn install → Store artifact in .m2



