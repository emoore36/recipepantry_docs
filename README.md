# Recipe Pantry
A web application for uploading and sharing recipes.

## Major Features
- Create and sign into an account.
- Upload and edit recipes.
- Edit and display user profile.
- Sort recipes into "shelves" by tags.
- Start and join communities to share recipes.
- Browse and save publicly-visible recipes from other users.

## Tools and Technologies
- [Frontend](https://github.com/emoore36/recipepantry_frontend): JavaScript via React via Next.js
- [Backend](https://github.com/emoore36/recipepantry_backend): Java via Spring Boot and Maven dependency service.
- Database: PostgreSQL via Docker image and container.

## Getting Started

### Prerequisites
Ensure you have the following software installed on your system:

- [Node 20.10.0 and npm 10.2.3](https://nodejs.org/en/download/current) for the frontend
- [Java 17.0.2](https://www.oracle.com/java/technologies/downloads/#java17), [Spring Boot 3.2.0](https://spring.io/blog/2023/11/23/spring-boot-3-2-0-available-now), and [Maven 3.8.6](https://maven.apache.org/download.cgi) for the backend
- [Docker CLI](https://docs.docker.com/get-docker/)

### Installation

1. Clone the Frontend Repository. 
    `git clone https://github.com/emoore36/recipepantry_frontend.git`
2. Install Frontend Dependencies. 
    ```
    cd recipepantry_frontend
    npm install
    ```
3. Clone the Backend Repository. 
    `git clone https://github.com/emoore36/recipepantry_backend.git`
4. Install Backend Dependencies and Run the Server.
    ```
    cd recipepantry_backend
    ./mvnw spring-boot:run
    ```
5. Set Up and Run the PostgreSQL Database using Docker. 
    `docker run -d -p 5432:5432 --name recipe_pantry_db -e POSTGRES_PASSWORD=mysecretpassword postgres`
6. Update Database Configurations.
   - Modify the database configurations in the backend application.properties file.
7. Start the frontend server. 
    `npm run dev`
8. Visit http://localhost:3000 in your browser.

## License
This project is open-source and available under the [MIT License](LICENSE). Feel free to use, modify, and distribute the code for your own purposes.
