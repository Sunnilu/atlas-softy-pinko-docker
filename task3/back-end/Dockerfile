# Use the official Python image
FROM python:3.9-slim

# Set the working directory
WORKDIR /app

# Install Flask-CORS
RUN pip3 install flask flask-cors

# Copy the rest of your application code
COPY . .

# Expose the port your app runs on
EXPOSE 5252

# Command to run your application
CMD ["python3", "api.py"]  # Adjust this according to your main application file
