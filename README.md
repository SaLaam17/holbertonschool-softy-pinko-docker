# Holberton School Softy Pinko Docker Project

## Project Overview

This project is designed to provide hands-on experience with Docker and Docker Compose. It focuses on creating, deploying, and scaling a full-stack application using Docker containers. The project covers aspects such as setting up front-end, back-end, proxy servers, and implementing horizontal scaling. Completed after the holberton v2 curriculum was implemented while tutoring.

## Tasks and Implementation

### Task 0: Create Your First Docker Image

- **Directory**: `task0`
- **Objective**: Create a Docker image based on Ubuntu, update and upgrade software, and echo "Hello, World!" on run.

### Task 1: Back-end

- **Directory**: `task1`
- **Objective**: Modify Dockerfile to install Python3, pip3, and Flask. Set up a Flask server that returns "Hello, World!" on a specific endpoint.

### Task 2: Front-end

- **Directory**: `task2`
- **Objective**: Set up a front-end environment using Nginx for static content hosting. Configure Nginx to serve the cloned Softy Pinko front-end.

### Task 3: Connecting the Front-end and Back-end

- **Directory**: `task3`
- **Objective**: Link the front-end to the back-end to display dynamic data. Implement CORS in Flask and modify the front-end to request data from the back-end.

### Task 4: Making it Simpler with Docker Compose

- **Directory**: `task4`
- **Objective**: Utilize Docker Compose to manage the multi-container setup. Include services for front-end, back-end, and proxy in the `docker-compose.yml` file.

### Task 5: Proxy Server
```task5/
├── docker-compose.yml
├── proxy/
│   ├── Dockerfile
│   └── default.conf
├── front-end/
│   ├── Dockerfile
│   ├── softy-pinko-front-end/...
│   └── softy-pinko-front-end.conf
├── back-end/
│   ├── Dockerfile
│   └── api.py
```
- **Directory**: `task5`
- **Objective**: Set up an Nginx proxy server to route requests to the front-end and back-end. Modify the application to route all traffic through the proxy server.

### Task 6: Scale Horizontally

- **Directory**: `task6`
- **Objective**: Implement horizontal scaling by running multiple instances of the API server. Configure load balancing using Nginx.

## Technologies Used

- Docker
- Docker Compose
- Nginx
- Flask (Python)
