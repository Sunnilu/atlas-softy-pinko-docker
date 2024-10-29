# Use the latest version of nginx
FROM nginx:latest

# Copy the softy-pinko-front-end files to the nginx HTML directory
COPY softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Copy the Nginx configuration file
COPY softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf

# Expose port 80
EXPOSE 80
