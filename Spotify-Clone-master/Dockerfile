# Use official Nginx image
FROM nginx:alpine

# Copy all project files to nginx html folder
COPY . /usr/share/nginx/html

# Replace default Nginx config
COPY nginx.conf /etc/nginx/conf.d/default.conf

# Expose website port
EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
