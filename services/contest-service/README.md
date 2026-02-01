# Contest Service

The "Brain" of the platform - manages all contest logic, including contest creation, scheduling, participant management, scoring, and leaderboards.

## Responsibilities

- Contest lifecycle management (create, start, end)
- Participant registration and management
- Real-time scoring and leaderboard updates
- Contest state management
- Integration with judge services for submission evaluation

## Technology

- Python FastAPI
- PostgreSQL database
- RabbitMQ for event-driven communication
- Real-time updates via WebSockets

## Structure

- `src/`: Python source code
- `Dockerfile`: Container build configuration
