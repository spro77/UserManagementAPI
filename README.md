# UserManagementAPI

This project is an ASP.NET Core Web API for managing users. It is designed for learning purposes and demonstrates:

- CRUD operations for user management
- Middleware for error handling, authentication, and logging
- Token-based authentication
- Standardized error responses

## How to Run

1. Restore dependencies:
   ```bash
   dotnet restore
   ```
2. Run the API:
   ```bash
   dotnet run
   ```

## API Endpoints

- `GET /users` - Retrieve all users
- `GET /users/{id}` - Retrieve a user by ID
- `POST /users` - Add a new user
- `PUT /users/{id}` - Update a user
- `DELETE /users/{id}` - Remove a user

## Authentication

All endpoints require a valid token in the `Authorization` header:
```
Authorization: Bearer valid-token
```

## Example cURL

```
curl -X GET http://localhost:5044/users -H "Authorization: Bearer valid-token"
```

## License

This project is for educational use only.

