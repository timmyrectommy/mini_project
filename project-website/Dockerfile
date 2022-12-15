# Use the official Ubuntu image as the base image
FROM ubuntu:latest

# Install Apache2 and necessary packages
RUN apt-get update && apt-get install -y apache2

WORKDIR /var/www/html/

# Copy the website files from the local directory
COPY . /var/www/html/

# Expose port 80 for incoming traffic
EXPOSE 80

# Start Apache2 when the container is run
CMD ["apachectl", "-D", "FOREGROUND"]
