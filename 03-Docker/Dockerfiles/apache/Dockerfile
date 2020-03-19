# Base Image. 
FROM ubuntu:16.04

# Owner of an Image
MAINTAINER Prasanto Dey <prasantodey8@gmail.com>

# Update Apt Repo.
RUN apt-get update 

# Install Apache Packages
RUN apt-get install apache2 -y 

# Cutome Page
COPY prasanto.html /var/www/html/index.html

# Expose Port Metadata Info
EXPOSE 80 3306

# Bring up the Apache Service
CMD ["/usr/sbin/apache2ctl","-D", "FOREGROUND"]
