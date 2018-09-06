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

