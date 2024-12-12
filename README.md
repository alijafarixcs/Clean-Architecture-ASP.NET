
# Clean-Architecture-ASP.NET Bookify
![Clean Architecture ASP.NET Bookify](https://github.com/alijafarixcs/Clean-Architecture-ASP.NET/blob/main/Graphics3.png?raw=true)
Bookify is a robust, scalable, and modular ASP.NET Core application designed to demonstrate modern software development principles. It incorporates Clean Architecture, Domain-Driven Design (DDD), Event-Driven Design, Command Query Responsibility Segregation (CQRS), Inversion of Control (IoC), and MediatR. This repository showcases how these concepts work together to build a high-quality, maintainable application.

---

## Key Features

1. **Clean Architecture**
   - Ensures separation of concerns.
   - Keeps the domain and application layers independent of external frameworks.

2. **Domain-Driven Design (DDD)**
   - Focuses on the core domain and domain logic.
   - Uses entities, value objects, aggregates, and repositories to model the domain.

3. **Event-Driven Design**
   - Utilizes domain events to decouple and improve scalability.
   - Supports asynchronous communication between components.

4. **CQRS (Command Query Responsibility Segregation)**
   - Separates read and write operations for better scalability and clarity.
   - Optimizes queries and commands independently.

5. **Inversion of Control (IoC)**
   - Promotes dependency injection for flexible and testable code.

6. **MediatR**
   - Simplifies the implementation of CQRS.
   - Manages the decoupling of request handling with commands and queries.

---

## Project Structure

```plaintext
Bookify/
├── Application/
│   ├── Commands/
│   ├── Queries/
│   ├── Interfaces/
│   └── Behaviors/
├── Domain/
│   ├── Entities/
│   ├── ValueObjects/
│   ├── Aggregates/
│   └── Events/
├── Infrastructure/
│   ├── Persistence/
│   ├── Services/
│   └── EventHandlers/
├── API/
│   ├── Controllers/
│   ├── Middlewares/
│   └── Configurations/
└── Shared/
    └── Utilities/
```

---

## Technologies Used

- **Framework:** ASP.NET Core
- **ORM:** Entity Framework Core , Dapper
- **Dependency Injection:** Built-in DI Container
- **MediatR:** For implementing CQRS and handling requests
- **Message Broker:** RabbitMQ (for event-driven communication)
- **Database:** SQL Server

---

## Getting Started

### Prerequisites

- .NET 8.0 SDK or later
- SQL Server
- RabbitMQ (for event-driven communication)

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/alijafarixcs/Clean-Architecture-ASP.NET.git
   cd Clean-Architecture-ASP.NET
   ```

2. Configure the connection strings in `appsettings.json` under the API project.

3. Run database migrations:
   ```bash
   dotnet ef database update --project Infrastructure
   ```

4. Start the application:
   ```bash
   dotnet run --project API
   ```

---

## Contributing

We welcome contributions! Please check out the [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---

## Contact

For questions or feedback, please contact Ali Jafari at [email@example.com](mailto:alijafarixcs@gmail.com).

