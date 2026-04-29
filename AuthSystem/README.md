# AuthSystem

A REST API authentication system built with C# ASP.NET Core and SQL Server.

## Features

- User registration with BCrypt password hashing
- User login with JWT token generation
- Protected routes using [Authorize] attribute
- Role-based access control (Admin / User)
- Entity Framework Core with SQL Server

## Tech Stack

- C# ASP.NET Core Web API
- Entity Framework Core
- SQL Server
- BCrypt.Net
- JWT (JSON Web Tokens)

## API Endpoints

| Method | Endpoint | Description | Auth Required |
|--------|----------|-------------|---------------|
| POST | /api/auth/register | Register a new user | No |
| POST | /api/auth/login | Login and get JWT token | No |
| GET | /api/auth/profile | Get current user profile | Yes |
| GET | /api/auth/admin | Admin only endpoint | Admin role |

## Getting Started

1. Clone the repository
2. Update appsettings.json with your SQL Server connection string
3. Run migrations: `dotnet ef database update`
4. Run the project: `dotnet run`
5. Open Swagger UI at `http://localhost:5118/swagger`