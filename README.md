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
```
https://docs.docker.com/engine/install/centos/

  sudo yum install -y yum-utils
   37  sudo yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo
   38  sudo yum install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
   39  docker ps
   40  systemctl status docker
   41  systemctl start docker
   42  clear
   43  docker -v

```
```

 ps -ef | grep docker
   49  clear
   50  docker ps
   51  docker ps -a
   52  docker images
   53  docker pull httpd
   54  docker images
   55  docker ps -a
   56  clear
   57  docker pull centos:7
   58  docker images
   59  clear
   60  docker create -dt --name c1 centos:7
   61  docker create -t --name c1 centos:7
   62  docker ps -a
   63  docker start c1
   64  docker ps -a
   65  docker run -dt  centos:7
   66  docker ps -a
   67  clear
   68  docker ps -a
   69  docker rm -f c1
   70  docker rm -f dreamy_cerf
   71  docker ps -a
   72  docker rmi -f httpd
   73  docker rmi -f centos:7
   74  clear
   75  docker run -h
   76  docker run --help
   77  clear
   78  docker run -it --name c1 centos:7
   79  docker ps
   80  docker ps -a
   81  docker start c1
   82  docker attach c1
   83  docker ps -a
   84  docker start c1
   85  clear
   86  docker run -dt --name c2 ubuntu
   87  docker ps
   88  docker attach c2
   89  clear
   90  history
   91  clear
   92  docker run -d --name c3 centos:7
   93  docker ps
   94  docker ps -a
   95  docker run -d --name c4 httpd
   96  docker ps
   97  docker attach c4
   98  clear
   99  ls
  100  docker ps
  101  docker ps -a
  102  docker start c4
  103  docker start c3
  104  docker ps -a
  105  docker ps
  106  docker exec -it c2 /bin/bash
  107  docker ps
  108  docker exec -it c4 /bin/bash
  109  clear
  110  docker ps -a
  111  docker stop c2
  112  docker kill c2
  113  docker ps
  114  docker rm c2
  115  docker rm -f c4
  116  docker ps
  117  docker ps -a
  118  docker ps

```
```

  ifconfig
  131  clear
  132  docker inspect c1
  133  docker ps -a
  134  docker start c1
  135  docker ps
  136  docker run -dit --name c2 centos:7
  137  docker ps
  138  docker inspect c2
  139  clear
  140  docker run -dt --name c4 redis
  141  docker ps
  142  docker exec -it c4 /bin/bash
  143  docker ps
  144  docker attach c4
  145  clear
  146  docker ps
  147  docker run -dt --name c5 httpd
  148  exit
  149  docker ps
  150  docker inpect c5
  151  docker inspect c5
  152  curl 172.17.0.5
  153  docker run -dit --name c6 nginx
  154  docker ps
  155  docker inspect c6
  156  curl 172.17.0.6
  157  clear
  158  docker ps
  159  docker rm -f `docker ps -aq`
  160  docker rmi -f `docker images`
  161  clear
  162  docker ps
  163  docker ps -a
  164  docker images
  165  docker run -dit --name web1 --hostname httpd -p 81:80 httpd
  166  docker ps
  167  docker inspect web1
  168  curl 172.17.0.2
  169  clear
  170  docker ps -a
  171  curl 172.31.28.36:81
  172  docker run -dit --name web2 -P nginx
  173  docker ps
  174  curl 172.31.28.36:32768


```
