# Use an official Python runtime as a parent image
FROM python:3.8-slim-buster

# Set the working directory in the container to /app
WORKDIR /app

# Copy requirements.txt into the container at /app
COPY requirements.txt .

# Update and install dependencies
RUN apt-get update && \
    apt-get install -y python3-pip && \
    pip3 install -r requirements.txt && \
    rm -rf /var/lib/apt/lists/*

# Copy the rest of the current directory contents into the container at /app
COPY . .

# Make port 9000 available to the world outside this container
EXPOSE 9000

# Define environment variable
ENV FLASK_APP=api.py

# Run api.py when the container launches
CMD ["python3", "-m", "flask", "run", "--host=0.0.0.0", "--port=9000"]

