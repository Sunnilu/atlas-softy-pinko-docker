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