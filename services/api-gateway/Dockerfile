FROM nginx:alpine

# Copy NGINX configuration
COPY nginx.conf /etc/nginx/nginx.conf
COPY src/ /usr/share/nginx/html/

# Expose ports
EXPOSE 80 443

# Start NGINX
CMD ["nginx", "-g", "daemon off;"]
