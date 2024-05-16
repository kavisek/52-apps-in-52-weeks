# Define the directory where your site will be served
SITE_DIR = /usr/local/var/www

# Define the main configuration file for nginx
NGINX_CONF = /usr/local/etc/nginx/nginx.conf

# Starts the development server
start:
	npm run dev

# Builds the project and copies files to the Nginx directory
build:
	npm run build
	cp -R dist/* $(SITE_DIR)

# Starts Nginx to serve the website
serve:
	sudo nginx -c $(NGINX_CONF)

# Stops Nginx
stop:
	sudo nginx -s stop

# Reloads Nginx configuration without downtime
reload:
	sudo nginx -s reload
