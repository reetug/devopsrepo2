# Use the official PHP image from Docker Hub
FROM php:latest

# Set the working directory in the container
WORKDIR /var/www/html

# Copy the current directory contents into the container
COPY . /var/www/html

# Install any additional dependencies if needed
RUN docker-php-ext-install mysqli pdo pdo_mysql

# Expose port 80
EXPOSE 80

# Start PHP's built-in web server
CMD ["php", "-S", "0.0.0.0:80", "-t", "/var/www/html"]

