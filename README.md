# YemekApp - Recipe Management Web App

A recipe management web application built with ASP.NET Core MVC (.NET 6) on a layered (N-tier) architecture.

## Features
- Recipe, ingredient, country and city management (CRUD)
- User registration, login and role-based access with cookie authentication
- Recipe report page with filtering, paging and ordering
- AJAX-driven dropdowns (country to city)

## Architecture
- AppCore: reusable base layer (generic Entity Framework repository, result models, paging/ordering, JWT utilities)
- DataAccess: Entity Framework Core entities, DbContext, repositories and SQL Server migrations
- Business: services and view models with validation
- YemekApp: ASP.NET Core MVC web UI (controllers and Razor views)

## Tech stack
C#, .NET 6, ASP.NET Core MVC, Entity Framework Core, SQL Server, Razor, JavaScript

## Run locally
1. Set the SQL Server connection string in YemekApp/appsettings.json
2. Run `dotnet ef database update` from the DataAccess project
3. Run `dotnet run` from the YemekApp project

Built during the Bilge Adam software development programme (2022).
