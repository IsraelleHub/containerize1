# your code goes here ...
# Use official Nginx base image
FROM nginx:latest

# Copy Nginx configuration file
COPY ./nginx/nginx.conf /etc/nginx/nginx.conf

# Copy SSL key pair
COPY ./nginx/files /etc/nginx/certs

# Expose ports
EXPOSE 80
EXPOSE 443

# Start Nginx
CMD ["nginx", "-g", "daemon off;"]
