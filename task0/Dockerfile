# based on the latest ubuntu
FROM ubuntu:latest

# Prevents interactive prompts during installations
ENV DEBIAN_FRONTEND=noninteractive

# Update APT using apt-get update
RUN apt-get update

# Upgrade currently installed software
RUN apt-get upgrade -y

# Declares the command to run when the container starts
CMD echo "Hello, World!"
