# Dot_Net_Core_API_Authentication_JWT

This repository contains an implementation of JWT (JSON Web Token) authentication in a .NET Core API project. The API demonstrates how to secure endpoints using JWT tokens, ensuring secure access to resources and providing a basic structure for implementing authentication in a .NET Core Web API.

## Features

- **JWT Authentication**: Secure API endpoints using JWT tokens.
- **User Authentication**: Login and registration functionality.
- **Bearer Token Authorization**: Protect endpoints by requiring a valid JWT token.

## Prerequisites

To run this project locally, you will need:

- **SQL Server** or a compatible database (e.g., SQLite) to store user data.
- **Postman** or any other API testing tool to test the authentication and API endpoints.

## Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/Dot_Net_Core_API_Authentication_JWT.git
cd Dot_Net_Core_API_Authentication_JWT
```

### 2. Install dependencies

```bash
dotnet restore
```

### 3. Set up the database

```bash
"ConnectionStrings": {
  "DefaultConnection": "Server=(localdb)\\mssqllocaldb;Database=JwtAuthDb;Trusted_Connection=True;"
}
```

### 4. Configure JWT Settings

```bash
"JwtSettings": {
  "SecretKey": "your_secret_key_here",
  "Issuer": "your_issuer_here",
  "Audience": "your_audience_here",
  "ExpirationMinutes": 60
}
```

### 5. Build and run the project
