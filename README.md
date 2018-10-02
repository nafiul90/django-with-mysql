# django-with-mysql


mysql config in system:

    mysql> USE mysql;
    mysql> CREATE USER 'YOUR_SYSTEM_USER'@'localhost' IDENTIFIED BY '';
    mysql> GRANT ALL PRIVILEGES ON *.* TO 'YOUR_SYSTEM_USER'@'localhost';
    mysql> UPDATE user SET plugin='auth_socket' WHERE User='YOUR_SYSTEM_USER';
    mysql> FLUSH PRIVILEGES;
    mysql> exit;

    $ service mysql restart
    
django congig:
    sudo apt-get install libmysqlclient-dev
    sudo apt-get install python-dev
    sudo python setup.py install
    Pip install django mysqlclient




