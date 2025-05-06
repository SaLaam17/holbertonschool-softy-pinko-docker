# based on the latest ubuntu
FROM nginx:latest

# Copy static website files
COPY softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Copy custom nginx config
COPY softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf
