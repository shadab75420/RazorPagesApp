# Razor Pages & Middleware Demo (.NET Core)

## Overview

This project is a .NET Core Razor Pages web application developed as part of the Wipro NGA .NET Cohort assignment. It demonstrates middleware configuration, static file handling, and Razor Pages routing.

---

## Features

- Razor Pages setup with proper routing  
- Static file serving from wwwroot  
- Middleware pipeline configuration  
- HTTPS redirection enabled  
- Multiple pages (Index, Privacy, Student)  

---

## Project Structure

RazorApp/

├── Pages/  
│   ├── Index.cshtml  
│   ├── Privacy.cshtml  
│   ├── Student.cshtml  
│   ├── Shared/  
│   ├── _ViewStart.cshtml  
│   └── _ViewImports.cshtml  

├── wwwroot/  
│   ├── css/  
│   ├── js/  
│   └── lib/  

├── Program.cs  
├── appsettings.json  
└── RazorApp.csproj  

---

## Setup and Run

### Prerequisites
- .NET SDK (6 or later)

### Run the project

dotnet run

### Open in Browser

Use the HTTPS URL shown in the terminal, for example:

https://localhost:7XXX/

---

## Application Routes

| Page     | URL        |
|----------|-----------|
| Home     | /         |
| Privacy  | /Privacy  |
| Student  | /Student  |

---

## Key Concepts

### Middleware

Configured in Program.cs:
- HTTPS Redirection
- Static Files
- Routing
- Authorization

### Razor Pages Routing

File-based routing is used:

Pages/Student.cshtml → /Student

### Static Files

Served from:

wwwroot/

Example access:

https://localhost:7XXX/css/site.css

---

## Sample Razor Page

@page
<h1>This is a student page</h1>

---

## Security

HTTPS is enforced using:

app.UseHttpsRedirection();

---

## Learning Outcomes

- Understanding middleware pipeline
- Razor Pages architecture
- Static file handling
- Routing in ASP.NET Core
