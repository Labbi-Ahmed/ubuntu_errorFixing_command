# ubuntu_errorFixing_command
This folder only contain the commend of error fixing all in ubuntu
#Mysql workbach connection problem : connection failed to mysql server with a user name
  solution: CREATE USER 'admin'@'localhost' IDENTIFIED BY 'password';
            GRANT ALL PRIVILEGES ON *.* TO 'admin'@'localhost' WITH GRANT OPTION;
