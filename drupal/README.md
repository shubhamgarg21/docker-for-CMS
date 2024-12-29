# Drupal with Docker

This setup provides a Drupal environment using Docker Compose, including:
- Drupal (latest version)
- MySQL 5.7 database

## Getting Started

1. Make sure you have Docker and Docker Compose installed on your system.
2. Clone or download this repository.
3. Navigate to the drupal directory.
4. Run the following command to start the containers:
   ```
   docker-compose up -d
   ```
5. Access Drupal installation at: http://localhost:8080

## Initial Setup

When you first access http://localhost:8080, you'll be guided through Drupal's installation process:

1. Choose your language
2. Choose "Standard" installation profile
3. For database configuration, use these settings:
   - Database type: MySQL
   - Database name: drupal
   - Database username: drupal
   - Database password: drupal_password
   - Host: db (important: use 'db' as the hostname)
   - Port: 3306

## Stopping the Environment

To stop the containers, run:
```
docker-compose down
```

## Data Persistence

All your Drupal files and database data are stored in Docker volumes, so your data will persist even after stopping the containers. 