# Docker for CRM Systems

A comprehensive Docker-based development environment for popular Content Management Systems (CMS). This repository provides ready-to-use Docker configurations for WordPress, Drupal, and Joomla.

## 🚀 Features

- Pre-configured Docker environments for three major CMS platforms:
  - WordPress (with MySQL 8.0)
  - Drupal (with PostgreSQL 16)
  - Joomla (with MySQL 8.0)
- Persistent data storage using Docker volumes
- Easy-to-use configurations with docker-compose
- Isolated environments for each CMS
- Port-mapped for local development

## 📋 Prerequisites

- Docker
- Docker Compose
- Git (for cloning the repository)

## 🛠 Installation & Setup

1. Clone the repository:
   ```bash
   git clone [your-repository-url]
   cd docker-for-CRM
   ```

2. Choose your preferred CMS directory:
   ```bash
   cd wordpress    # for WordPress
   # OR
   cd drupal       # for Drupal
   # OR
   cd joomla       # for Joomla
   ```

3. Start the containers:
   ```bash
   docker-compose up -d
   ```

## 💻 Usage

### WordPress Setup
- Access WordPress at: http://localhost:8080
- Database Configuration:
  - Database: wordpress
  - Username: wordpress
  - Password: wordpress
  - Host: db:3306

### Drupal Setup
- Access Drupal at: http://localhost:8080
- Database Configuration:
  - Database: drupal
  - Username: drupal
  - Password: drupal_password
  - Host: db
  - Port: 5432

### Joomla Setup
- Access Joomla at: http://localhost:8080
- Database Configuration:
  - Database: joomla
  - Username: joomla
  - Password: joomla_password
  - Host: db

## 🛑 Stopping the Environment

To stop any of the environments:
```bash
docker-compose down
```

To stop and remove all data (including database):
```bash
docker-compose down -v
```

## 📁 Directory Structure

```
docker-for-CRM/
├── wordpress/
│   ├── docker-compose.yml
│   └── README.md
├── drupal/
│   ├── docker-compose.yml
│   └── README.md
└── joomla/
    ├── docker-compose.yml
    └── README.md
```

## 🔒 Security Notes

- Default passwords in the configuration files are for development purposes only
- Change all default passwords before using in a production environment
- Keep your Docker and CMS versions updated

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the [GNU General Public License v3.0](LICENSE).