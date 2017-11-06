# mysql修改密码的方法
***

1、 SET PASSWORD
```
mysql -uroot -p
SET PASSWORD FOR 'root'@'localhost'=PASSWORD('newpassword')；
```

2、mysqladmin
```
无密码的情况下
mysqladmin -uroot password "newpassword"
有密码的情况下
mysqladmin -uroot password oldpassword "newpassword"
```

3、 UPDATE
use mysql
UPDATE user SET password = PASSWORD('newpassword')WHERE user='root';
FLUSH PRIVILEGES;

4、 忘记root密码情况
mysqld_safe --skip-grant-tables&
mysql -uroot 
UPDATE user SET password = PASSWORD('newpassword')WHERE user='root';
FLUSH PRIVILEGES;

