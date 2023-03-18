# ubuntu_errorFixing_command
This folder only contain the commend of error fixing all in ubuntu
#Mysql workbach connection problem : connection failed to mysql server with a user name
  solution: CREATE USER 'admin'@'localhost' IDENTIFIED BY 'password';
            GRANT ALL PRIVILEGES ON *.* TO 'admin'@'localhost' WITH GRANT OPTION;
            

Job for mysql.service failed because the control process exited with error code. See "systemctl status mysql.service" and "journalctl -xeu mysql.service" for details.
solution: 

        sudo apt autoremove --purge mysql-server\* mariadb-server\*
        sudo rm -rf /var/lib/mysql
        sudo rm -rf /etc/mysql/
        sudo mkdir -p /etc/mysql/conf.d
        sudo apt install mysql-server
