
# LibraryWebAPI - Backend Service

This is a RESTful Web API built using ASP.NET Core to manage a small library system. It provides endpoints for handling books, borrowers, and loan transactions. The project also supports JWT-based authentication for secure access.

## Features

- User Registration & Login with JWT Authentication
- CRUD operations for Books and Borrowers
- Book issuing and returning
- Overdue loan tracking
- Protected routes accessible only by authenticated users
- Code-First database modeling using Entity Framework Core

## Technologies Used

- ASP.NET Core Web API
- Entity Framework Core (Code First)
- SQL Server (or LocalDB)
- JWT for authentication
- Git & GitHub for version control

## API Endpoints

### Authentication

- `POST /api/auth/register` – Register a new user
- `POST /api/auth/login` – Login and receive JWT token

### Books API

- `GET /api/books` – List all books
- `GET /api/books/{id}` – Get book by ID
- `POST /api/books` – Add a new book
- `PUT /api/books/{id}` – Update book details
- `DELETE /api/books/{id}` – Delete a book

### Borrowers API

- `GET /api/borrowers` – List all borrowers
- `POST /api/borrowers` – Add a new borrower
- `PUT /api/borrowers/{id}` – Update borrower info
- `DELETE /api/borrowers/{id}` – Delete a borrower

### Loans API

- `POST /api/loans` – Issue a book to a borrower
- `POST /api/returns` – Return a borrowed book
- `GET /api/loans/overdue` – Get all overdue loans

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/LibraryWebAPI.git
   ```
2. Open the solution in Visual Studio or VS Code.
3. Update the `appsettings.json` with your SQL Server connection string.
4. Run the following commands in the terminal:
   ```bash
   dotnet ef database update
   dotnet run
   ```
5. Use Swagger or Postman to interact with the API.

## Bonus (Optional Frontend)

If implemented, a minimal frontend allows:
- Viewing books
- Issuing and returning loans

## Team Members

[name             id
1. nuredin seid   1501419
2. leul tekeste   1501318
3. selamawit asfaw 1501459
4. selamawit girma 1501458

]

## License

This project is for educational purposes only.
