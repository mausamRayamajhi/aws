# AWS with Microservices
Aws integration with spring boot.


# Important Command in linux

<details><summary> Command</summary>
<p>

- Present working directory

```
pwd
```

- To make root user

```
sudo -i
```

- Central repo list

```
yum repolist
```

- Show all the list of already installed software/packages

```
yum list installed
```

- Show packages as group

```
yum gruoplist
```

- To install the package

```
yum install <package name> 
```

- To start the service

```
service httpd start
```

- To server the page

```
vi /var/www/html/index.html
```

- To stop the service

```
service httpd stop
```

- To remove the package

```
yum remove httpd 
```

- To see log from last 5 line

```
tail -5 /var/log/yum.log 
```

- To search

```
yum search java
```

</p>

</details>

# Install MYSQL in AWS

```
yum install -y mariadb-server

systemctl enable mariadb

systemctl start mariadb

mysql_secure_installation

mysql -uroot -p
```

# Install Java

```
yum install java-1.8.0-openjdk

alternatives --config java
```

# To Make Spring Project Run Automatically When Instance Is Running

```
cat /ect/rc.local
cp coupon-0.1-SNAPSHOT.jar /home/ec2-user/
vi /etc/rc.local
java -jar /home/ec2-user/coupanservice-0.1-SNAPSHOT.jar
chmod +x /etc/rc.d/rc.local
```

# Packages changed in aws 
```
amazon-linux-extras install epel -y
yum install stress -y
```
