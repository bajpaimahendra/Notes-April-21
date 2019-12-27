### Install LAMP with one command - Linux Apache MySQL PHP( current version 7) -----

	https://help.ubuntu.com/community/ApacheMySQLPHP
	http://howtoubuntu.org/how-to-install
	https://gregrickaby.com/2013/05/how-to-install-lamp-on-ubuntu/

	sudo apt-get install lamp-server^	(	^ means using tasksel	)
	sudo chmod -R 777 /var/www
	sudo a2enmod rewrite				( load rewrite modile )

	sudo /etc/init.d/apache2 restart	( restart apache )

### Check Loaded Module) ---------
		apache2ctl -M

### Install curl --------------------------------------------
	sudo apt-get install curl
	curl --version    ( check version )

### Install lDap module of php --------
   sudo apt-get install php7.0-ldap
   sudo /etc/init.d/apache2 restart ( restart apache )
   to get the php configuration phpinfo();

### Additional PHP modules-----------

	sudo apt install php-curl php-gd php-mbstring php-mcrypt php-xml php-xmlrpc php-json


### Install the Memcached --------------
	http://www.liquidweb.com/kb/how-to-install-the-memcached-php-extension-on-ubuntu-14-04-lts/
	1- sudo apt-get install php-memcached
	OR
	sudo apt-get install php5-memcached

	2- sudo apt-get install memcached
	3- restart apache

### Run Multiple Version of php ==============================================================
	https://www.tecmint.com/install-different-php-versions-in-ubuntu/
    	sudo apt-get install python-software-properties

   	sudo add-apt-repository ppa:ondrej/php

   	sudo apt-get update

    	sudo apt-get install php7.1

    $ sudo a2dismod php7.0
    $ sudo a2enmod php5.6
    $ sudo /etc/init.d/apache2 restart

### Install MongoDB --------------------------------------
	1- https://docs.mongodb.com/manual/tutorial/install-mongodb-on-ubuntu/
	2- php monngo driver
		sudo apt-get install php5-mongo
		sudo gedit /etc/php5/apache2/php.ini
		and extension=mongo.so in php.ini





