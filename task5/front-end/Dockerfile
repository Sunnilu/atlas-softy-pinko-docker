# Use the latest Nginx image as the base
FROM nginx:latest

# Copy the web application files into the Nginx default directory
COPY softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Copy the Nginx configuration file into the container at /etc/nginx/conf.d/default.conf
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf

# Assuming this is part of your Dockerfile for the back-end or front-end service
COPY requirements. txt.

