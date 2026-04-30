# TaskManagerAPI

A REST API for managing tasks built with C# ASP.NET Core and SQL Server.

## Features

- Create, Read, Update and Delete tasks
- Task priority levels (High, Medium, Low)
- Task completion status tracking
- Entity Framework Core with SQL Server

## Tech Stack

- C# ASP.NET Core Web API
- Entity Framework Core
- SQL Server

## API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | /api/tasks | Get all tasks |
| GET | /api/tasks/{id} | Get task by ID |
| POST | /api/tasks | Create a new task |
| PUT | /api/tasks/{id} | Update a task |
| DELETE | /api/tasks/{id} | Delete a task |

## Getting Started

1. Clone the repository
2. Update appsettings.json with your SQL Server connection string
3. Run migrations: `dotnet ef database update`
4. Run the project: `dotnet run`
5. Open Swagger UI at `http://localhost:5110/swagger`