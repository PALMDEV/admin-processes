FROM ubuntu:16.04 as dev

#installing  dependencies
RUN apt update && apt install -y curl && curl -sL https://deb.nodesource.com/setup_8.x 
RUN apt install -y nodejs && apt install -y npm
RUN npm install -g @angular/cli
RUN npm install -g n
RUN n 8

# Install Nginx.
# RUN \
#   add-apt-repository -y ppa:nginx/stable && \
#   apt update && \
#   apt install -y nginx && \
#   rm -rf /var/lib/apt/lists/* && \
#   echo "\ndaemon off;" >> /etc/nginx/nginx.conf && \
#   chown -R www-data:www-data /var/lib/nginx

ENV API_URL http://localhost:5000
ENV API_KEY THISISAENVARIABLE

EXPOSE 8008 
EXPOSE 4200

# FROM dev as build



# FROM dev as prod
