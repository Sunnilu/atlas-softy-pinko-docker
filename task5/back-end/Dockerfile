# Use the latest version of Nginx
FROM nginx:latest

# Copy the proxy configuration file to the correct location
COPY proxy.conf /etc/nginx/conf.d/default.conf

# Expose port 80
EXPOSE 80
# Use the latest version of Ubuntu as a parent image
FROM ubuntu:22.04

#update the package lists for upgrades for packages that need upgrading
RUN apt-get update

#upgrade all the installed packages
RUN apt-get upgrade -y

#install Flask using pip3
RUN pip3 install flask

WORKDIR  /app

COPY . /app

EXPOSE 5252

CMD ["python3", "api.py"]