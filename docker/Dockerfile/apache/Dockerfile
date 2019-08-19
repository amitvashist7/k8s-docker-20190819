# Base Image
FROM ubuntu:16.04

# Owner
MAINTAINER Amit Vashist <amitvashist7@gmail.com>

# Update my APT Repo.
RUN apt-get update

# Install Apache Packages
RUN apt-get install apache2 -y

# Create a Test Web Page
RUN echo "Hello World" > /var/www/html/index.html

# Copy Info web pages
COPY info.html /var/www/html/

# Expose 
EXPOSE 80 

# Bring the Apache Service 
CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]
