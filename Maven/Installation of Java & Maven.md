<h1 align="center"> ☆ Installation of Java & Maven in Amazon Linux 2023 ☆</h1>


&nbsp;&nbsp;&nbsp;&nbsp;• **Java must be installed before Maven.**

**➤ Update System Packages :**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; `sudo yum update -y`

**➤ Search Available Java Versions :** 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; `dnf search corretto` 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Purpose: Displays all available Amazon Corretto Java versions.

**➤ Copy the Package Name :** 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;✦ Copy the package name before `.x86_64`

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;✦ Example: `java-23-amazon-corretto-headless`

**➤ Install Java :** 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; `sudo dnf install -y PASTE_THE_VERSION_PACKAGE_NAME`

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;✦ Example: `sudo dnf install -y java-23-amazon-corretto-headless`

**➤ Verify Java Installation :**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; `java -version`

**➤ Install Maven :**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; `sudo yum install maven -y`

**➤ Verify Maven Installation :**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; `mvn --version`




| Command | Purpose | Note |
|---|---|---|
| `sudo yum update -y` | Checks for updates and installs the latest available packages. | Update System Packages |
|`dnf search corretto`| Lists all available JDK versions | Displays all available Amazon Corretto Java versions.  |
||Copy the Package Name|Copy the package name before `.x86_64`. Example: java-23-amazon-corretto-headless|
|`sudo yum install JDK_VERSION -y`	|Installs Java on the system.|Install Java|
|`java --version`|Checks whether Java is installed successfully.|Verify Java Installation. <br> `Expected Output:` </br>• openjdk 17.x.x|
|`sudo yum install maven -y`|Installs Apache Maven|Install Maven|
|`mvn --version`|Checks whether Maven is installed successfully|Verify Maven Installation <br>  `Expected Output:` </br> • Apache Maven 3.x.x <br> • Java version: 17.x.x </br> |

<b>Note :</b>


  
