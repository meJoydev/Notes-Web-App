# Notes Management System

- This is a fullstack application developed using ASP.NET core web API for backend services and JavaScript, HTML, and CSS for frontend interactions.

- A Notes application where you can Create, Read, Update, and Delete your notes.

- Integrated Fetch API for frontend-backend communication and utilized Postman & Swagger UI for API testing and documentation.

- Optimized API performance using asynchronous programming (async/await) and secured endpoints with CORS policies.

## Features

- Full CRUD REST API for notes (create, read, update, delete)
- EF Core **code-first migrations** — schema is generated from C# model classes
- **Swagger UI** for interactive API documentation and testing
- Frontend built with the **Fetch API** as a single-page app, with async error handling on every request

## Tech stack

**Backend:** `ASP.NET Core Web API` · `Entity Framework Core` · `SQL Server` · `Swagger`
**Frontend:** `JavaScript (Fetch API)` · `HTML5` · `CSS3`

## Project structure

```
NotesApp/
  Controllers/     API endpoints (NotesController)
  Models/          Note entity
  Data/            EF Core DbContext, migrations
  wwwroot/         Static frontend (HTML/CSS/JS)
```

## Getting started

**Prerequisites:** .NET SDK, SQL Server (Express/LocalDB works).

```bash
git clone https://github.com/meJoydev/Notes-Web-App.git
cd Notes-Web-App
dotnet restore
```

Update the connection string in `appsettings.json`, then:

```bash
dotnet ef database update
dotnet run
```

Open the Swagger UI at the URL shown in the console, or open `wwwroot/index.html` to use the frontend directly.

## Roadmap

- [ ] Add user accounts so notes are private per user
- [ ] Add search/filter on the frontend

## License

MIT
