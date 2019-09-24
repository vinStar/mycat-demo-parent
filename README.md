# mycat-demo-parent
mycat对mysql数据库进行分库分表demo

## 环境
1. linux jdk 1.8   
2. mycat 1.6  
3. `vim /etc/profile` add `MYCAT_HOME=/usr/local/mycat` in the end 
4.  `vi      /etc/sysconfig/network`  追加一行： `HOSTNAME=你的主机名  ` used for  》schema 》dataHost
5. `vi     /etc/hosts` 127.0.0.1               `localhost.localdomain localhost 你的主机名` used for  》schema 》dataHost  
6. docker 》mysql  `<writeHost host="mycat1" url="127.0.0.1:3306" user="root" password="123456" />` don't use `localhost` for mysql which mean use socket connect in localhost

>  [root@bogon mycat]# mysql  

>  ERROR 2002 (HY000): Can't connect to local MySQL server through socket '/var/lib/mysql/mysql.sock' (2)

  
