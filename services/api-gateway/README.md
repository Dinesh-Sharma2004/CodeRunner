# API Gateway Service

The API Gateway serves as the single entry point for all client requests. It handles routing, load balancing, authentication, rate limiting, and request/response transformation.

## Technology

- NGINX for reverse proxy and load balancing
- Request routing to appropriate microservices
- SSL/TLS termination
- Rate limiting and security policies

## Structure

- `src/`: Source code and configuration files
- `Dockerfile`: Container build configuration
- `nginx.conf`: NGINX configuration file
