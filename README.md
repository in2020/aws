# aws
## connect to ec2 on terminal
```
ssh -i my-ec2-key-pair.pem ec2-user@<EC2-INSTANCE-PUBLIC-IP-ADDRESS>
```
## docker install on ec2
- (https://www.ybrikman.com/writing/2015/11/11/running-docker-aws-ground-up/)
```
[ec2-user]$ sudo yum update -y
[ec2-user]$ sudo yum install -y docker
[ec2-user]$ sudo service docker start
[ec2-user]$ sudo usermod -a -G docker ec2-user
[ec2-user]$ exit
reconnect
```
## Amazon Linux 2 AMI 에 PHP, Python, Ruby 배포 환경 구성
- (https://www.lesstif.com/pages/viewpage.action?pageId=51283065)
```
amazon-linux-extras install python3 php7.2 nginx1.12 redis4.0
yum install php-cli php-common php-gd php-mbstring  php-mysqlnd php-pdo php-fpm php-xml php-opcache php-zip
```
