# Joomla Docker Setup

This setup provides a quick way to get Joomla CMS running using Docker.

## Prerequisites
- Docker
- Docker Compose

## Getting Started

1. Start the containers:
   ```bash
   docker-compose up -d
   ```

2. Access Joomla:
   - Open your browser and go to `http://localhost:8080`
   - Follow the Joomla installation wizard
   - For database configuration, use:
     - Database Type: MySQL
     - Host Name: joomladb
     - Username: joomla
     - Password: joomla_password
     - Database Name: joomla

3. Stop the containers:
   ```bash
   docker-compose down
   ```

Note: Your Joomla files and database data will persist in Docker volumes even after stopping the containers. 