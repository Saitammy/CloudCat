## CloudCat

### Overview
This repository contains a Category Controller for managing categories in the CloudCat application. The controller is built using ASP.NET Core and Entity Framework Core for database operations.

### Features
- **Index**: Displays a list of categories.
- **Create**: Creates a new category.
- **Edit**: Modifies an existing category.
- **Delete**: Removes a category from the database.

### Getting Started
1. Clone the repository to your local machine.
2. Open the solution in Visual Studio or your preferred IDE.
3. Configure the `ApplicationDbContext` in `Startup.cs` to connect to your database.
4. Run the migrations to create the necessary database schema:

```dotnet ef migrations add InitialCreate```
```dotnet ef database update```

5. Build and run the application.

### Usage
1. Navigate to the Category section in the CloudCat application.
2. **Index**: View the list of existing categories.
3. **Create**: Add a new category by providing a name and display order.
4. **Edit**: Modify the details of an existing category.
5. **Delete**: Remove a category from the database.

### Dependencies
- **ASP.NET Core**: Provides the framework for building web applications.
- **Entity Framework Core**: Used for database operations and ORM.
- **Microsoft.AspNetCore.Mvc**: Handles HTTP requests and responses.
- **CloudCat.Data**: Contains the `ApplicationDbContext` for database interactions.
- **CloudCat.Models**: Defines the `Category` model for category data.

### Notes
- Ensure that the database connection string is correctly configured in `appsettings.json`.
- This controller uses `TempData` to display success messages after creating, editing, or deleting categories.

Feel free to contribute, report issues, or suggest improvements!
