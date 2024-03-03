jenkins installation:
=====================

## Prerequisites:
* 4 GB Ram
* 50 GB drive space

## Jenkins installation steps:
  For install jenkins you should install java, jave is prerequisites for jenkins installation then you install jenkins.

# steps:
---------
```
sudo apt update
sudo apt install openjdk-17-jdk -y
sudo wget -O /usr/share/keyrings/jenkins-keyring.asc \
  https://pkg.jenkins.io/debian/jenkins.io-2023.key
echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \
  https://pkg.jenkins.io/debian binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null
sudo apt-get update
sudo apt-get install jenkins
sudo systemctl status jenkins

```

```
sudo cat /var/lib/jenkins/secrets/initialAdminPassword
```


when we install jenkins server it will create user as jenkins 
and jenkins home directory is /var/lib/jenkins




  
