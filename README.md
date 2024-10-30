Spring Petclinic Application

Application Overview

The Spring Petclinic application is a sample project that demonstrates the use of the Spring framework in a veterinary clinic management context. It allows users to add information about pet owners, pets, veterinarians, and appointment scheduling. This serves as a foundational example of CRUD operations in web applications.

Repository Contents
This repository includes all necessary components to run the application using Docker and Docker Compose:

backend/ - The Spring Boot application handling business logic and database connections.

frontend/ - The Angular application that provides the user interface.

postgres/ - Docker configuration for the PostgreSQL database, which stores application data.

docker-compose.yml - A file that enables the launch of all services (frontend, backend, database) with a single Docker command.


Running the Application
Before starting the application, ensure Docker and Docker Compose are installed on your machine.

Clone the repository and navigate to the directory:

git clone https://github.com/AhmedHadzihamdo/petclinic_app_dockerized.git

cd <repository_name>

Start the application using the Docker Compose command:
docker compose up

Once all services are running, the frontend should be accessible at http://localhost:80, and the backend API at http://localhost:9966.

Additional Notes
Database Configuration: PostgreSQL credentials (username, password, database name) are set up in docker-compose.yml. You can adjust these settings in the Docker Compose file or directly in the backend application’s application.properties file.
Docker Network: The application uses a Docker network to facilitate communication between services.
