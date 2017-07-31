# LAMO-on-RaspberryPi

make sure update

    sudo apt-get update
    sudo apt-get upgrade
install Apache

    apt-get install apache2 apache2-utils
install PHP5

    apt-get install libapache2-mod-php5 php5 php-pear php5-xcache
install php5 MySQL database support

    apt-get install php5-mysql
install MySQL

    apt-get install mysql-server mysql-client
Set the root password during the installation

install phpmyadmin

    apt-get install phpmyadmin
Choose Apache2 when webServer is asked

During the installation the MySQL root password will be asked
Config Apache2 for phpmyadmin

    nano /etc/apache2/apache2.conf
Use Ctrl + V to turn to last line of the edit page and add:

    Include /etc/phpmyadmin/apache.conf
Save and restart Apache2 by command:

    /etc/init.d/apache2 restart
Done phpMyAdmin will be at : http://x.x.x.x/phpmyadmin
