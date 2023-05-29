```

creation of server :

ami : 
CentOS 7 (x86_64) - with Updates HVM

ins type :
t2.medium

root storage : 20gb

```

```

login to server 


sudo -i
yum update -y

--- for jenkins insallaion :

https://pkg.jenkins.io/redhat-stable/

----


    5  yum install wget -y
    6  sudo wget -O /etc/yum.repos.d/jenkins.repo https://pkg.jenkins.io/redhat-stable/jenkins.repo
    7  sudo rpm --import https://pkg.jenkins.io/redhat-stable/jenkins.io-2023.key
    8  yum install fontconfig java-11-openjdk
    9  yum install jenkins
   10  systemctl status jenkins
   11  systemctl start jenkins
   13  cat /var/lib/jenkins/secrets/initialAdminPassword
   17  chkconfig jenkins on

```
