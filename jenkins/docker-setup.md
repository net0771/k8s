## Install Docker
```sh
yum install.md docker

systemctl start docker

systemctl enable docker
```

## 젠킨스 서버의 젠킨스 사용자에게 도커에 액세스할 수 있는 권한 제공
```sh
  sudo groupadd docker
  
  sudo usermod -aG docker jenkins
  
  sudo chmod 777 /var/run/docker.sock
  
```
## sudo 액세스 권한을 얻으려면 Jenkins 사용자를 sudoers 파일에 추가
```sh
   vi /etc/sudoers
   
   jenkins ALL=(ALL) NOPASSWD: ALL
```   
   

