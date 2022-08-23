1) install nginx : sudo apt-get install nginx
2) goto cd /etc/nginx
3) nginx.conf is the main file where http context includes our servers.
4) write server configurations inside /sites-available folder. like static-server.config, this server config will included automatically inside http context in nginx.conf file
5) copy static-server.config file inside /sites-enabled folder, coz all the files inside /sites-enabled will attached in nginx as it is included inside nginx.conf file
