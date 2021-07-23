First install fcgiwrap:<br>
Command:<br>
sudo apt install fcgiwrap<br>
sudo cp /usr/share/doc/fcgiwrap/examples/nginx.conf /etc/nginx/fcgiwrap.conf<br>
cd /etc/nginx/sites-available<br>

Now add following line:<br>
server {<br>
listen 80 default_server;<br>
include /etc/nginx/fcgiwrap.conf;<br>

Then, restart server using sudo service nginx restart<br>
The /etc/nginx/fcgiwrap.conf fi le places the CGI root at the default
directory location of /usr/lib/cgi-bin/. A simple script can be created
at that location<br>
Linux command:<br>
sudo mkdir /usr/lib/cgi-bin/

sudo cp dht /usr/local/bin
cd /usr/lib/cgi-bin/  
sudo chown root:root dht  
sudo chmod ugo+s dht  
ls -l dht  
-rwsr-sr-x 1 root root 9360 Oct 11 15:36 dht
