# Based on the latest Ubuntu
FROM ubuntu:latest

# Avoid interactive prompts
ENV DEBIAN_FRONTEND=noninteractive

# Update and upgrade
RUN apt-get update && apt-get upgrade -y

# Install Python, pip, and venv
RUN apt-get install -y python3 python3-pip python3-venv

# Create a virtual environment
RUN python3 -m venv /opt/venv \
 && /opt/venv/bin/pip install --upgrade pip \
 && /opt/venv/bin/pip install flask flask-cors

# Make the venv the default Python path
ENV PATH="/opt/venv/bin:$PATH"

# Set working directory and copy app
WORKDIR /app
COPY api.py /app/api.py

# Expose the Flask port
EXPOSE 5252

# Run the Flask app
CMD ["python", "api.py"]
