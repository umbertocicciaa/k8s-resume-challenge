# Use a base image that includes MariaDB
# Use the official MariaDB image as the base image
FROM mariadb:latest

# Set environment variables
ENV MARIADB_ROOT_PASSWORD=password123
ENV DB_NAME=ecomdb
ENV DB_USER=ecomdb-user
ENV DB_PASSWORD=password123

# Copy the schema file into the Docker container
COPY db-load-script.sql /docker-entrypoint-initdb.d/

# Expose the port
EXPOSE 3306