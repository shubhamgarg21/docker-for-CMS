# WordPress Docker Setup

This is a Docker-based WordPress development environment.

## Prerequisites

- Docker
- Docker Compose

## Getting Started

1. Make sure Docker and Docker Compose are installed on your system
2. Clone this repository
3. Run the following command in the project directory:
   ```bash
   docker-compose up -d
   ```
4. Access WordPress at: http://localhost:8080

## Configuration

- WordPress site will be available at `http://localhost:8080`
- MySQL Database:
  - Database: wordpress
  - Username: wordpress
  - Password: wordpress
  - Root Password: somewordpress

## Stopping the Environment

To stop the containers, run:
```bash
docker-compose down
```

To stop the containers and remove all data (including database), run:
```bash
docker-compose down -v
``` 