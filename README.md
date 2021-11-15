# Java11 Installation on Ubuntu20.04

This is a guide for Java installation on Ubuntu 20.04

## Step 1 - Install Java with Apt

Update the server and install java 11 using Apt package manager

```
sudo apt-get update
Sudo apt-get install openjdk-11-jdk
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

Add the following text to [java.sh](http://java.sh) file and save&#x20;

```
#/bin/bash
export JAVA_HOME=/usr/lib/jvm/java-11-openjdk-amd64

```



