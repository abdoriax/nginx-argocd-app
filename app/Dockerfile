# Use the official NGINX image from Docker Hub
FROM nginx:1.25-alpine

# Remove default NGINX welcome page
RUN rm /usr/share/nginx/html/index.html /usr/share/nginx/html/50x.html

# Copy our custom HTML file to the NGINX web root directory
COPY ./index.html /usr/share/nginx/html/index.html

# Expose port 80 to the outside world
EXPOSE 80

# Command to run NGINX when the container starts
CMD ["nginx", "-g", "daemon off;"]
