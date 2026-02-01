# Universal Contest Platform

A comprehensive monorepo for a universal contest platform supporting Data Structures & Algorithms, Machine Learning, and Cybersecurity challenges.

## Architecture

This platform follows a microservices architecture with the following components:

### Services

- **API Gateway**: Single entry point using NGINX for routing and load balancing
- **Auth Service**: User authentication, authorization, and role management
- **Contest Service**: Core contest logic, scheduling, and leaderboard management
- **Problem Service**: Problem repository for DSA, ML, and Cyber challenges
- **Judge Services**: Specialized execution engines
  - `judge-standard`: C++/Python execution for DSA problems
  - `judge-cyber`: Scapy-based packet analysis for cybersecurity challenges
  - `judge-ml`: Papermill-based notebook evaluation for ML challenges

### Frontend

- **Creator Studio**: Admin interface for contest and problem management
- **Contest Arena**: Participant interface for competing in contests

### Infrastructure

- Kubernetes manifests for orchestration
- ELK Stack for centralized logging
- Prometheus for monitoring and alerting

## Tech Stack

- **Backend**: Python (FastAPI)
- **Frontend**: React
- **Infrastructure**: Docker, Kubernetes
- **Message Queue**: RabbitMQ
- **Database**: PostgreSQL
- **Communication**: gRPC, REST APIs

## Getting Started

1. Start all services using Docker Compose:
   ```bash
   docker-compose up -d
   ```

2. Access services:
   - API Gateway: http://localhost
   - Frontend: http://localhost:3000
   - RabbitMQ Management: http://localhost:15672

## Project Structure

```
coderunner/
├── common/              # Shared libraries and contracts
├── infrastructure/     # K8s, monitoring, logging configs
├── services/           # Microservices
│   ├── api-gateway/
│   ├── auth-service/
│   ├── contest-service/
│   ├── problem-service/
│   ├── judge-standard/
│   ├── judge-cyber/
│   ├── judge-ml/
│   └── frontend/
└── docker-compose.yml  # Local development setup
```

## Development

Each service contains its own `Dockerfile` and `src/` directory. Refer to individual service README files for specific setup instructions.
