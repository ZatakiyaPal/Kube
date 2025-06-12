# Step 1: Use Nginx base image
FROM nginx:latest

# Step 2: Remove default nginx web files
RUN rm -rf /usr/share/nginx/html/*

# Step 3: Copy your static website files to Nginx's web directory
COPY . /usr/share/nginx/html

# Step 4: Expose port 80
EXPOSE 80

# Step 5: Start Nginx in foreground
CMD ["nginx", "-g", "daemon off;"]