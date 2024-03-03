Sample Maven Project Build:
===========================

# Sample maven project github link:
Below is the sample maven hello world sample project

```
https://github.com/jenkins-docs/simple-java-maven-app.git

```
# check the git is installed or not
```
git --version

```
# Install openjdk17 in ubuntu:
```
sudo apt update
sudo apt install openjdk-17-jdk -y

```

# Installation of maven 3.9.x:

```
cd /opt

sudo wget https://dlcdn.apache.org/maven/maven-3/3.9.6/binaries/apache-maven-3.9.6-bin.tar.gz

sudo tar -xvf apache-maven-3.9.6-bin.tar.gz
sudo ln -s /opt/apache-maven-3.9.6 /opt/maven

sudo vi /etc/profile.d/maven.sh

export M2_HOME=/opt/maven
export MAVEN_HOME=/opt/maven
export PATH=${M2_HOME}/bin:${PATH}
sudo chmod +x /etc/profile.d/maven.sh

source /etc/profile.d/maven.sh
mvn -v
```

# Build Sample project:
```
git clone https://github.com/jenkins-docs/simple-java-maven-app.git
cd simple-java-maven-app/
mvn package
cd /home/ubuntu/simple-java-maven-app/target/
sudo java -jar my-app-1.0-SNAPSHOT.jar

```
above jar will print the hello world
