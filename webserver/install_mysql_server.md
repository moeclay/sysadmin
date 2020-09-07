### Install MySQL Client & Server
```
# apt install mysql-client-core-5.7
# apt install mysql-server
# mysql_secure_installation
```

### Buat User MySQL
```
$ mysql -u root -p
> CREATE USER 'sammy'@'%' IDENTIFIED BY 'password';
> GRANT ALL PRIVILEGES ON *.* TO 'sammy'@'%' WITH GRANT OPTION;
> exit;

$ mysql -u sammy -p -h 192.168.4.45
```

### Akses Service & Allow Firewall
```
$ systemctl status mysql.service

# ufw allow 3306
# ufw disable
# ufw enable
```
