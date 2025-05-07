# Use latest Ubuntu as base image
FROM ubuntu:latest

# Update and upgrade packages
RUN apt-get update && \
    apt-get upgrade -y

# Install Python3, pip3
RUN apt-get install -y python3 python3-pip

# Handle potential "externally managed" error
RUN rm -f /usr/lib/python*/EXTERNALLY-MANAGED

# Install flask and cors using pip3
RUN pip3 install flask flask-cors

# Set the working directory
WORKDIR /app

# Copy the Flask application
COPY api.py .

# Command to run the Flask server
CMD ["python3", "api.py"]
