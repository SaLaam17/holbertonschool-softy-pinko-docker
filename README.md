Creating a README.md file for the Docker project.
task0:
```Dockerfile:
# based on the latest ubuntu
FROM ubuntu:latest

# Prevents interactive prompts during installations
ENV DEBIAN_FRONTEND=noninteractive

# Update APT using apt-get update
RUN apt-get update

# Upgrade currently installed software
RUN apt-get upgrade -y

# Declares the command to run when the container starts
CMD echo "Hello, World!"```

creating docker image:
```docker build -f ./Dockerfile -t softy-pinko:task0 .````

running container:
```docker run -it --rm --name softy-pinko-task0 softy-pinko:task0```

