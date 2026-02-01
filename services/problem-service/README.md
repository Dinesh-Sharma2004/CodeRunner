# Problem Service

Manages all contest problems including DSA (Data Structures & Algorithms), Machine Learning, and Cybersecurity challenges.

## Responsibilities

- Problem CRUD operations
- Problem metadata management (difficulty, tags, categories)
- Test case storage and management
- Problem versioning
- Problem templates and starter code

## Technology

- Python FastAPI
- PostgreSQL database for metadata
- Object storage (S3/MinIO) for large files and test cases

## Structure

- `src/`: Python source code
- `Dockerfile`: Container build configuration
