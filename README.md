# 🐳 Docker SonarQube 🔍

## 🎯 SonarQube Project with Docker

The goal of this project is to set up an environment with SonarQube and PostgreSQL using Docker. This project is based on the video ["Installing and Configuring SonarQube with Docker Compose"](https://www.youtube.com/watch?v=HSFHgti6nXg) from my YouTube channel.

## 🛠️ Services Created

- **📊 SonarQube**: A tool for continuous code analysis.
- **💾 PostgreSQL**: A database used by SonarQube to store data.

## 🔐 Environment Variables

### SonarQube

- `SONAR_JDBC_URL`: JDBC connection URL for the PostgreSQL database.
- `SONAR_JDBC_USERNAME`: Username to access the database.
- `SONAR_JDBC_PASSWORD`: Password to access the database.

### PostgreSQL

- `POSTGRES_USER`: Username for the PostgreSQL database.
- `POSTGRES_PASSWORD`: Password for the PostgreSQL database.
- `POSTGRES_DB`: Name of the database to be used by PostgreSQL.

## 💽 Volumes

- `sonar_data`: Stores SonarQube data persistently.
- `sonar_logs`: Stores SonarQube logs persistently.
- `sonar_db`: Stores PostgreSQL database data persistently.

## 🚀 Running the Project

To create and start the services defined in the `compose.yaml` file, use the following command:

```bash
docker compose up -d
```

## ℹ️ Additional Notes

- Ensure Docker and Docker Compose are installed on your system before running the project.
- For more details on configuring SonarQube, refer to the [official documentation](https://docs.sonarqube.org/).
- If you encounter any issues, check the logs stored in the `sonar_logs` volume for troubleshooting.

---
