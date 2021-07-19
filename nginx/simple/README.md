Configuring an Nginx Web Server
Nginx can be confi gured using the fi les in /etc/nginx/ where the core confi
guration fi les are as follows:

■ nginx.conf is the main confi guration fi le for the server.

■ The sites-available directory contains the confi guration fi les for any
virtual sites, and the sites-enabled directory should contain a symbolic
link to a confi guration fi le in the sites-available directory, to activate
a site.

Most of the confi guration changes are performed on the default
fi le entry in the sites-available directory.

In addition to the confi guration fi les, the functionality of Nginx can be further
extended (e.g., to provide Python support) with the use of modules. You
can identify the current modules that have been compiled into Nginx using
the following:

pi@erpi ~ $ nginx -V

nginx version: nginx/1.6.2

TLS SNI support enabled ...

Creating Web Pages and Web Scripts
To create a simple web page for the RPi web server, you can use the nano editor
and some basic HTML syntax as shown in index.html file
