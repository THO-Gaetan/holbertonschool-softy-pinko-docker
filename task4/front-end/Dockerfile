FROM nginx:latest

# Copy the softy-pinko-front-end files to the nginx html directory
COPY ./softy-pinko-front-end/ /var/www/html/softy-pinko-front-end/

# Copy the Nginx configuration file
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf

# Set the port to 9000
EXPOSE 9000