<h1 align="center"> ☆ Installation of Java & Maven in Linux ☆</h1>

| Command | Purpose | Note |
|---|---|---|
| sudo yum update -y | Checks for updates and installs the latest available packages. | Update System Packages |
|sudo yum search jdk| Lists all available JDK versions | Always select the JDK version. The version name will include “JDK”, for example: openjdk-17-jdk. |
|sudo yum install <span title="Select the Java version."> `jdk_version` -y	|Installs Java on the system.|Install Java|
|java --version|Checks whether Java is installed successfully.|Verify Java Installation. <br> `Expected Output:` </br>• openjdk 17.x.x|
|sudo yum install maven -y|Installs Apache Maven|Install Maven|
|mvn --version|Checks whether Maven is installed successfully|Verify Maven Installation <br>  `Expected Output:` </br> • Apache Maven 3.x.x <br> • Java version: 17.x.x </br> |

<b>Note :</b>

&nbsp;&nbsp;&nbsp;&nbsp;• Java must be installed before Maven.
