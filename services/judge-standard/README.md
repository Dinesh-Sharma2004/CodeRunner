# Judge Standard Service

Execution engine for standard programming problems (DSA) supporting C++ and Python.

## Responsibilities

- Code compilation and execution in isolated containers
- Test case validation
- Resource limit enforcement (CPU, memory, time)
- Security sandboxing
- Result reporting back to contest service

## Technology

- Python FastAPI
- Docker for code execution isolation
- C++ compiler (g++)
- Python interpreter
- Resource monitoring and limits

## Structure

- `src/`: Python source code
- `Dockerfile`: Container build configuration
