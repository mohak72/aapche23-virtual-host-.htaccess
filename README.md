# aapche23-virtual-host-.htaccess

<VirtualHost *:80>
        ServerName  www.orangemantra.com
        ServerAdmin webmaster@localhost
        DocumentRoot /var/www/html

    <Directory "/var/www/html">
        Options FollowSymLinks Includes
        AllowOverride All
        Order allow,deny
        Allow from all
    </Directory>

        ErrorLog ${APACHE_LOG_DIR}/error.log
        CustomLog ${APACHE_LOG_DIR}/access.log combined

</VirtualHost>
