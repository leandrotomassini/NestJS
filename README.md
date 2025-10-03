<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>

# Teslo API

This repository contains the backend API for the Teslo shop, built with NestJS. It provides endpoints for product management, authentication, and file uploads.

---

## Prerequisites

- Node.js
- Yarn
- Docker

---

## Installation

1.  **Clone the project**
    ```bash
    git clone <repository-url>
    ```

2.  **Install dependencies**
    ```bash
    yarn install
    ```

3.  **Set up environment variables**
    Clone the `.env.template` file and rename it to `.env`.
    ```bash
    cp .env.template .env
    ```
    Update the variables in the `.env` file with your configuration (e.g., database credentials, JWT secret).

4.  **Start the database**
    Run the following command to start the PostgreSQL database using Docker.
    ```bash
    docker-compose up -d
    ```

---

## Running the Application

-   **Development mode:**
    ```bash
    yarn start:dev
    ```
    The application will be available at `http://localhost:3000`.

-   **Production mode:**
    ```bash
    yarn start:prod
    ```

---

## Running Tests

-   **Run all tests:**
    ```bash
    yarn test
    ```

-   **Run end-to-end tests:**
    ```bash
    yarn test:e2e
    ```

---

## API Seed

To populate the database with initial data, send a `GET` request to the following endpoint after the application is running:

```
http://localhost:3000/api/seed
```

---

*Developed by ltomassini*