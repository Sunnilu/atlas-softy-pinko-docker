# Use an official Python runtime as a parent image
FROM ubuntu:22.04

# Set the working directory in the container to /app
WORKDIR /app

# Update and install dependencies
RUN apt-get update && \
    apt-get install -y python3 python3-pip && \
    rm -rf /var/lib/apt/lists/*

# Copy the current directory contents into the container at /app
COPY . /app

# Install Flask using pip3
RUN pip3 install Flask

# Make port 5252 available to the world outside this container
EXPOSE 5252

# Define environment variable
ENV FLASK_APP=api.py

# Run api.py when the container launches
CMD ["python3", "-m", "flask", "run", "--host=0.0.0.0", "--port=5252"]
