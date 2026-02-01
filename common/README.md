# Common Shared Library

This directory contains shared code, contracts, and schemas used across all microservices in the Universal Contest Platform.

## Structure

- **protos/**: gRPC protocol buffer definitions for inter-service communication
- **events/**: RabbitMQ message schemas and event definitions for asynchronous communication

## Usage

Services should import and use these shared definitions to ensure consistency across the platform.
