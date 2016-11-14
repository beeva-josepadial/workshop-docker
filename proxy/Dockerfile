FROM nginx:1.11.5-alpine

MAINTAINER genDevOps

# Clean default sites
RUN rm -rf /etc/nginx/sites-enabled

# Add config
COPY config/nginx.conf /etc/nginx/conf.d/default.conf

# Add ssl certs
COPY ssl/nginx.crt /etc/nginx/ssl/nginx.crt
COPY ssl/nginx.key /etc/nginx/ssl/nginx.key

# Ports
EXPOSE 443
