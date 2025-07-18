# Car Parking Management System

A modular, layered Car Parking Management System built using ASP.NET Core (.NET 8), Entity Framework Core, and SQL Server. The solution follows clean architecture principles to separate concerns across API, Business Logic, Database, UI (Web & Desktop), and Test projects.
---
## Solution Structure
CarParking.sln
│
Api/ # ASP.NET Core Web API (RESTful endpoints),
Business/ # Business logic layer (services, interfaces),
BusinessTest/ # Unit tests for business layer,
Database/ # EF Core DbContext, Models, Views, and Migration logic,
DBTest/ # Integration or unit tests for database logic,
Desktop/ # Desktop UI client (e.g., WinForms or WPF),
Web/ # ASP.NET Core MVC or Razor Pages frontend.

## Technologies Used

- **.NET 8**
- **ASP.NET Core Web API**
- **Entity Framework Core (8.0.11)**
- **SQL Server**
- **Razor Pages / MVC (optional)**
- **xUnit / NUnit / MSTest** for testing
- **Dependency Injection**
- **Clean/Layered Architecture**

---

## Database Project (`Database/`)

### `CarParkingContext`

The main `DbContext` used across the system.

#### 📦 Dependencies

- `Microsoft.EntityFrameworkCore` (v8.0.11)
- `Microsoft.EntityFrameworkCore.SqlServer` (v8.0.11)

#### DbSets (Tables)

- `UserInfo`
- `Role`
- `CarCategory`
- `Slot`
- `SlotBook`
- `PaymentMethod`
- `Payment`
- `ClientCar`

#### Setup (Command Promt)
1. Clone the repository
    git clone https://github.com/shadi-islam/aspnet-practice-edge
    cd aspnet-practice-edge
2. Restore NuGet packages
   dotnet restore
3. Apply EF Core migrations
   Navigate to the Database/ folder: dotnet ef database update
4. Run the API
   cd Api
   dotnet run






