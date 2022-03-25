# Java11 Installation on Ubuntu20.04

This is a guide for Java installation on Ubuntu 20.04

## Step 1 - Install Java with Apt

Update the server and install java 8 using Apt package manager

```
sudo apt-get update
sudo apt-get install openjdk-8-jdk
```

## Step 2 - Find JDK Installation Directory

```
update-alternatives --config java
```

## Step 3 - Configure Environment Variables

You need to configure the environment variables for JAVA\_HOME

```
sudo nano /etc/profile.d/java.sh
```

Add the following text to [java.sh](http://java.sh) file and save (JAVA\_HOME="your java installation directory which you get from step2")

```
#/bin/bash
export JAVA_HOME=/usr/lib/jvm/java-11-openjdk-amd64

```

## Step 4 - Test Your Installation

You can test your installation by asking java version to your server.

```
java --version
```

The output should be like the following image;

![](.gitbook/assets/image.png)
