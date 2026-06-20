## **Apache Tomcat Installation in Amazon Linux**

### **Dependency**

✦ **Dependency for Tomcat and Maven:** JDK (Java Development Kit)

✦ Tomcat and Maven require Java to run.

---

### **Update Packages Before Installing Applications**

```bash
sudo yum update -y
```

### **Install Java**

```bash
sudo yum install java-11-amazon-corretto-headless
```

---

### **Install Tomcat**

1. Open Google.
2. Search:

```text
tomcat 8.0.52 download index
```

3. Open:

```text
https://archive.apache.org/dist/tomcat/tomcat-8/v8.0.52/bin/
```

4. Right-click on:

```text
apache-tomcat-8.0.52.tar.gz
```

and copy the link.

5. Download Tomcat:

```bash
sudo wget PASTE_THE_URL
```

6. Verify the file:

```bash
ls
```

7. Extract the file:

```bash
tar -xvf TOMCAT_FILENAME
```

8. Enter the Tomcat directory:

```bash
cd FOLDER_NAME
```

9. Go to the bin directory:

```bash
cd bin/
```

10. Check the current path:

```bash
pwd
```

11. Copy the displayed path.

---

### **Configure Environment Variables**

Open the profile file:

```bash
sudo vi /etc/profile
```

Go to the bottom, press `o`, and add:

```bash
export CATALINA_HOME=PASTE_PWD_PATH
export PATH=$PATH:PASTE_PWD_PATH
```

**Note:**

* Remove `/bin` from `CATALINA_HOME`.
* Do not remove `/bin` from `PATH`.

**Example:**

```bash
export CATALINA_HOME=/home/ec2-user/apache-tomcat-8.0.52
export PATH=$PATH:/home/ec2-user/apache-tomcat-8.0.52/bin
```

Save and exit:

```text
Esc
:wq!
```

Apply the variables:

```bash
export CATALINA_HOME=/home/ec2-user/apache-tomcat-8.0.52
export PATH=$PATH:/home/ec2-user/apache-tomcat-8.0.52/bin
```

---

### **Verify Tomcat Installation**

```bash
sh version.sh
```

---

### **Start Tomcat**

```bash
startup.sh
```

If you see a message indicating Tomcat started successfully, the installation is working.

---

### **Stop Tomcat**

```bash
shutdown.sh
```
-----

### **Verify Tomcat Installation in Browser**

✦ We can check whether Tomcat is installed and running by accessing it from a web browser.

---

### **Configure Security Group**

1. Open the EC2 Instance.
2. Click **Security**.
3. Click **Security Groups**.
4. Click **Edit Inbound Rules**.
5. Click **Add Rule**.

Enter:

```text
Type   : Custom TCP
Port   : 8080
Source : Anywhere-IPv4
```

6. Click **Save Rules**.

---

### **Access Tomcat in Browser**

1. Copy the **Public IP Address** of the EC2 Instance.
2. Open a new browser tab.
3. Enter the Public IP Address along with the Tomcat port number.

**Default Tomcat Port:**

```text
8080
```

**Example:**

```text
13.232.183.75:8080
```

or

```text
http://13.232.183.75:8080
```

---

### **Expected Result**

If the Tomcat welcome page appears, Tomcat is installed and running successfully.

---

### **Short Note**

✦ Tomcat can be verified through a web browser using the server's Public IP Address and port number.

✦ The default Tomcat port number is `8080`.

✦ Port `8080` must be allowed in the Security Group Inbound Rules.
