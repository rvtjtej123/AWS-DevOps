**JohnCena**
kane
djs jg sgb sgsd

# Maven Notes

This is **bold**

This is *italic*

Run `mvn clean install`

~~~
git clone
~~~
<h1 align="center"> </h1>


<h1 align="center"> ☆ Installation of Java & Maven in Amazon Linux 2023 ☆</h1>

<h3 align="center"> **★ NOTE: Java must be installed before Maven.** </h3>
<br><br>

**➤ Update System Packages :**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; `sudo yum update -y`


&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Purpose: Displays all available Amazon Corretto Java versions.

**➤ Copy the Package Name :** 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;✦ Copy the package name before `.x86_64`

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;✦ Example: `java-23-amazon-corretto-headless`

**➤ Install Java :** 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; `sudo dnf install -y PASTE_THE_VERSION_PACKAGE_NAME`

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;✦ Example: `sudo dnf install -y java-23-amazon-corretto-headless`



<h1 align="center"> </h1>

**<h3><br>✦ There are different package variants for Amazon Corretto 23 (Java 23):</br></h3>**

| Package | Purpose |
|---|---|
| java-23-amazon-corretto | Full Java Development Kit (JDK). Includes compiler (javac), runtime (java), and development tools. This is what most developers install. |
|java-23-amazon-corretto-headless|JDK without GUI/X11 components. Smaller footprint, ideal for servers, containers, Spring Boot apps, Jenkins, etc.|
|java-23-amazon-corretto-devel|Development tools package (compiler, headers, etc.). Often pulled in automatically by the main JDK package.|


<h1 align="center"> ☆ Introduction of Maven ☆</h1>

<h2 align="left"> ➤ Maven Build Lifecycle </h2>

&nbsp;&nbsp; ● Maven uses the **JDK (Java Development Kit)** to compile and build Java applications.

&nbsp;&nbsp; ● Maven cannot run without Java being installed.

<h1 align="center"> * Extra *</h1>   
   
| Command | Purpose | What it does |
|---|---|---|
`mvn clean install` | Most common real-world command. | <ul><li>Full Clean Build</li> <li>Deletes old build</li>  <li>Compiles project </li>  <li>Runs tests </li> <li>Packages artifact <li>Installs into local repo </li></ul>
