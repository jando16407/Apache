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

If not, make one.