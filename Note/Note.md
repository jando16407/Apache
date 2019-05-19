# Apache Note


## Apache setting up on Mac OSX


### Check Apache version

Apache comes with MacOSX by default.
Check the version by typing

		httpd -v

### Running on MacOS

* To start running apache server

		sudo apachectl start

* To stop running

		sudo apachectl stop

* To restart

		sudo apachectl restart

### Setting up root directory

Default directoey is /Library/WebServer/Documents

Apache users folder is /etc/apache2/users/

Move to users folder and check if you have a config file named after username such as

		yourusername.conf

If not, make one and add below code to the conf file.

		<Directory "/Users/YourUsername/Sites/">
            Options Indexex MultiViews
            AllowOverride All
            Order allow, deny
            Allow from all
		</Directory>

Change access mode to give apache access

		sudo chmod 644 YourUserName.conf

Restart Apache by typing

		sudo apachectl restart