# installing jenkins in Ubuntu 
1. download the Repository 
```
  curl -fsSL https://pkg.jenkins.io/debian-stable/jenkins.io.key | sudo tee \
    /usr/share/keyrings/jenkins-keyring.asc > /dev/null
```

2.Then add a Jenkins apt repository entry:
```
 echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \
    https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
    /etc/apt/sources.list.d/jenkins.list > /dev/null
```

- Update the system 
```
sudo apt-get update

```
- Installing openjdk:
```
  sudo apt-get install fontconfig openjdk-11-jre
```
- Installing the jenkins
```
  sudo apt-get install jenkins
```

- check the jenkins is running or not
```
systemctl status jenkins 

systemct enable jenkins
```
