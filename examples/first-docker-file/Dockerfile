# Use an official Python image as the base image
FROM python:3.9-slim

# Set the working directory in the container
WORKDIR /app

# Copy application files into the container
COPY requirements.txt /app
COPY devops /app/devops

# Install dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Expose the application port
EXPOSE 8000

# Command to run the application
CMD ["python3", "devops/manage.py", "runserver", "0.0.0.0:8000"]
