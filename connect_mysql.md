# Connect WSL's MySQL from Windows Host Machine

mysql installation:
- `sudo apt update && sudo apt upgrade`
- `sudo apt install mysql-server`
- `mysql --varsion`

start mysql server:
- `sudo service mysql start`

set the root user password to some value:
- `sudo my sql`
- `ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'password';`
- `FLUSH PRIVILEGES;`

initialize other parameters of mysql db server:
- `sudo mysql_secure_installation -p`

now you can open mysql using this command:
- `sudo mysql -u root -p`

changing the default port:
- `sudo nano /etc/mysql/my.cnf`

add these lines:
- [mysqld]
- port = 33069

restart the server and set the service to be auto-loaded:
- `sudo service mysql restart`
- `sudo update-rc.d mysql defaults`
