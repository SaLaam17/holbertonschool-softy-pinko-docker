# based on the latest ubuntu
FROM ubuntu:latest

# Prevents interactive prompts during installations
ENV DEBIAN_FRONTEND=noninteractive

# Update APT using apt-get update
RUN apt-get update

# Upgrade currently installed software
RUN apt-get upgrade -y

# install Python3 and pip3
RUN apt-get install -y python3 python3-pip

# Install Flask with pip3
RUN pip3 install flask

# Set working directory
WORKDIR /app

# Copy the Flask app into the image
COPY api.py /app/api.py

# Expose port 5252 (used by Flask)
EXPOSE 5252

# Declares the command to run when the container starts
CMD echo "Hello, World!"
