# NestJS Modular Monolith CQRS Event Sourcing Architecture Template 🚀

![GitHub release](https://img.shields.io/github/release/aligcgl/nestJS-modular-monolith-cqrs-event-sourcing-architecture-template.svg)
![GitHub stars](https://img.shields.io/github/stars/aligcgl/nestJS-modular-monolith-cqrs-event-sourcing-architecture-template.svg)
![GitHub forks](https://img.shields.io/github/forks/aligcgl/nestJS-modular-monolith-cqrs-event-sourcing-architecture-template.svg)

Welcome to the **NestJS Modular Monolith CQRS Event Sourcing Architecture Template**. This repository provides a scalable NestJS project template that supports modular monolith architecture, CQRS (Command Query Responsibility Segregation), and Event Sourcing. Built with Domain-Driven Design (DDD) and Onion Architecture principles, this template is ideal for developing proof-of-concept (PoC) projects and production-ready backend systems.

## Table of Contents

- [Features](#features)
- [Technologies](#technologies)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Releases](#releases)

## Features

- **Modular Monolith Architecture**: Organize your codebase into distinct modules for better maintainability.
- **CQRS Support**: Separate read and write operations for improved performance and scalability.
- **Event Sourcing**: Store state changes as a sequence of events, allowing for better auditing and recovery.
- **Domain-Driven Design**: Focus on the core domain and its logic, improving communication and collaboration among team members.
- **Onion Architecture**: Promote a clean separation of concerns and dependency management.
- **Flexible Database Support**: Choose from MongoDB, PostgreSQL, SQLite, or other databases as per your requirements.
- **Docker and Docker Compose**: Easily deploy your application using containerization.

## Technologies

This template incorporates a variety of technologies to enhance functionality and performance:

- **NestJS**: A progressive Node.js framework for building efficient, reliable, and scalable server-side applications.
- **CQRS**: Command Query Responsibility Segregation pattern for separating read and write operations.
- **Event Sourcing**: Storing state changes as a sequence of events.
- **MongoDB**: A NoSQL database for high-performance data storage.
- **Kafka**: A distributed streaming platform for building real-time data pipelines.
- **EventStoreDB**: A database specifically designed for event sourcing.
- **PostgreSQL**: An open-source relational database.
- **SQLite**: A lightweight database engine.
- **TypeScript**: A superset of JavaScript that compiles to plain JavaScript.

## Getting Started

To get started with this template, clone the repository and install the dependencies. Follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/aligcgl/nestJS-modular-monolith-cqrs-event-sourcing-architecture-template.git
   ```

2. Navigate into the project directory:

   ```bash
   cd nestJS-modular-monolith-cqrs-event-sourcing-architecture-template
   ```

3. Install the dependencies:

   ```bash
   npm install
   ```

4. Set up your environment variables. Create a `.env` file based on the provided `.env.example` file.

5. Start the application:

   ```bash
   npm run start:dev
   ```

Your application should now be running on `http://localhost:3000`.

## Project Structure

The project is organized into several key directories:

```
src/
├── modules/             # Contains feature modules
│   ├── users/           # User module
│   ├── products/        # Product module
│   └── orders/          # Order module
├── shared/              # Shared utilities and constants
├── infrastructure/      # Infrastructure-related code (database, messaging)
└── main.ts              # Entry point of the application
```

### Modules

Each module contains its own controllers, services, and entities. This separation allows for easier testing and maintenance.

### Shared

The shared directory includes common utilities, constants, and interfaces that can be used across different modules.

### Infrastructure

This directory contains the configuration for databases, messaging systems, and other infrastructure components.

## Usage

To utilize this template effectively, consider the following:

1. **Define your domain**: Identify the core business logic and domain entities that your application will manage.

2. **Create modules**: Structure your application into modules based on the domain entities. Each module should encapsulate its own logic and dependencies.

3. **Implement CQRS**: Separate your commands (writes) and queries (reads) to optimize performance and maintainability.

4. **Utilize Event Sourcing**: Implement event sourcing to track changes in your application state. This allows for better auditing and the ability to replay events if needed.

5. **Deploy with Docker**: Use Docker and Docker Compose for deployment. Create a `docker-compose.yml` file to define your services and run them with a single command.

## Contributing

Contributions are welcome! If you would like to contribute to this project, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them.
4. Push your branch to your forked repository.
5. Create a pull request describing your changes.

Please ensure that your code adheres to the project's coding standards and is well-documented.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Releases

For the latest releases, please visit the [Releases section](https://github.com/aligcgl/nestJS-modular-monolith-cqrs-event-sourcing-architecture-template/releases). You can download and execute the latest files from there.

---

This README provides a comprehensive overview of the NestJS Modular Monolith CQRS Event Sourcing Architecture Template. Use it as a guide to navigate the project and make the most of its features.