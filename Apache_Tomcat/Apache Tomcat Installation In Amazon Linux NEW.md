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

1. Open Google and search:

```text
tomcat 9 download
```

2. Open:

```text
tomcat.apache.org/download-90.cgi
```

3. Copy the download link of:

```text
Core → tar.gz
```

4. Download Tomcat:

```bash
wget PASTE_THE_URL
```

5. Extract the downloaded file:

```bash
tar -xvf TOMCAT_NAME
```

6. Rename the Tomcat folder:

```bash
mv OLD_FOLDER_NAME NEW_FOLDER_NAME
```

7. Copy the Tomcat folder to `/opt`.

**Why `/opt`?**

✦ The `/opt` directory is commonly used for third-party software installations.

```bash
sudo cp -r FOLDER_NAME /opt
```

8. Go to the `/opt` directory:

```bash
cd /opt
```

9. Check the owner of the folder:

```bash
ls -l
```

10. Change the owner from `root` to `ec2-user`:

```bash
sudo chown -R NEW_USERNAME:NEW_USERNAME TOMCAT_FOLDER_NAME
```

**Example:**

```bash
sudo chown -R ec2-user:ec2-user apache-tomcat-9
```

11. Verify the ownership change:

```bash
ls -l
```
-----------
----------
----------

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
