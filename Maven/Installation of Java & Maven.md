<h1 align="center"> ☆ Installation of Java & Maven in Amazon Linux 2023 ☆</h1>

<h3 align="center"> **★ NOTE: Java must be installed before Maven.** </h3>
<br><br>

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


<h1 align="center"> </h1>

**<h3><br>✦ There are different package variants for Amazon Corretto 23 (Java 23):</br></h3>**

| Package | Purpose |
|---|---|
| java-23-amazon-corretto | Full Java Development Kit (JDK). Includes compiler (javac), runtime (java), and development tools. This is what most developers install. |
|java-23-amazon-corretto-headless|JDK without GUI/X11 components. Smaller footprint, ideal for servers, containers, Spring Boot apps, Jenkins, etc.|
|java-23-amazon-corretto-devel|Development tools package (compiler, headers, etc.). Often pulled in automatically by the main JDK package.|
|java-23-amazon-corretto-debugsymbols|Debug symbols used for low-level debugging with tools like gdb. Rarely needed.|
|java-23-amazon-corretto-javadocs|Offline Java API documentation. Not needed unless you want local docs.|
|java-23-amazon-corretto-jmods|Java module files used by tools such as jlink to create custom runtimes. Advanced use case.|


