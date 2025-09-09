# Use the official Nginx image 
FROM nginx:latest

# Copy front-end files into Docker image
COPY softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Copy Nginx configuration into Docker image
COPY softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf

# Expose port 9000
EXPOSE 9000