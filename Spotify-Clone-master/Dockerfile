# Stage 1: Build React app
FROM node:20-alpine AS build

# Copy all project files to nginx html folder
COPY . /usr/share/nginx/html

COPY . .
RUN npm run build

# Replace default Nginx config
COPY nginx.conf /etc/nginx/conf.d/default.conf

EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
