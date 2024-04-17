# CRUD Smart Catalog Films 

The project involved the implementation of JWT (JSON Web Tokens) in an application designed to manage a film catalog using ASP.NET Core MVC, WebAPI, and XUnit for testing. To achieve a well-structured and maintainable codebase, I adopted the CQRS (Command Query Responsibility Segregation) and MediatR patterns, while adhering to Clean Architecture and Domain-Driven Design (DDD) principles. 

![image](https://github.com/bccampos/smartfilms/assets/36283909/8b707be3-de6c-4b85-a444-4b0fa3246966)


## How to use and run the project

Open the solution and build the application. After the successful build run, you can create the SmartCatalogFilms using the script in the main folder or you can run the command migration update-database. 
```bash
update-database
```
Also you will need to startup 3 projects (MVC / API / Identity.API)
![image](https://github.com/bccampos/smartfilms/assets/36283909/16efc3c2-bd43-4034-aea7-29a52fb4a004)

## :hammer:  API Core

![image](https://github.com/bccampos/smartfilms/assets/36283909/f600dae8-cde6-45b3-8df0-f83eecfb79e3)

- `Application`: Commands e Command Handler / Queries (Using EF)
- `Domain`: Entities / Value Objects / Interfaces / Validation 
- `Infrastructure`: Context EF / Repositories / Mappings / Migrations

## XUnit - Tests cover some business rules requirements 
![image](https://github.com/bccampos/smartfilms/assets/36283909/bc38301b-4e9e-4209-8669-b6697a6b8701)

## Swagger Catalog Films API ( with authorized configurated ) 
![image](https://github.com/bccampos/smartfilms/assets/36283909/6c9bbd20-a5a3-46e3-b74f-65eb6cbef748)

## Swagger Identity API 
![image](https://github.com/bccampos/smartfilms/assets/36283909/ffaf846a-0bae-442b-9640-8ed5805fcc42)

## MVC UI
> **_NOTE:_** The application has a user-friendly approach where the "List All" functionality is open for everyone to access without requiring authentication. However, when users click on a film to view its details, the system prompts them to log in for added security. Once logged in, users gain access to additional features such as adding new films, editing existing ones, removing films, and obtaining comprehensive film details.

### Before authentication
![image](https://github.com/bccampos/CRUDSmartFilms/assets/36283909/29fcea91-e5da-4930-9c9b-c14b5bca77ab)

### Login
![image](https://github.com/bccampos/CRUDSmartFilms/assets/36283909/bf641f0a-0956-48da-b6f2-998d3ec7a1bf)

### After authentication
![image](https://github.com/bccampos/CRUDSmartFilms/assets/36283909/78b412ce-0f76-4b63-9aaf-641e6513958d)

### Films details
![image](https://github.com/bccampos/CRUDSmartFilms/assets/36283909/2828ffba-f690-49ae-8d65-c410a51f4126)


  


