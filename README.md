# Books API

This is a simple RESTful API built with Golang and MongoDB. It allows users to perform CRUD operations on a collection of books.

## Deployment
The API is deployed on **Railway** and can be accessed at:

**Base URL:** `https://goapi-production-7230.up.railway.app`

## Endpoints

### Get All Books
**GET** `/books`

#### Response:
```json
[
  {
    "id": 1,
    "name": "The Alchemist",
    "author": "Paulo Coelho",
    "quantity": 10
  },
  ...
]
```

### Get a Single Book
**GET** `/books/{id}`

#### Response:
```json
{
  "id": 1,
  "name": "The Alchemist",
  "author": "Paulo Coelho",
  "quantity": 10
}
```

### Create a Book
**POST** `/books`

#### Request Body:
```json
{
  "id": 69,
  "name": "New Book",
  "author": "John Doe",
  "quantity": 5
}
```

#### Response:
```json
{
  "message": "Book created successfully"
}
```

### Update a Book
**PUT** `/books/{id}`

#### Request Body:
```json
{
  "name": "Updated Book",
  "author": "Jane Doe",
  "quantity": 7
}
```

#### Response:
```json
{
  "message": "Book updated successfully"
}
```

### Delete a Book
**DELETE** `/books/{id}`

#### Response:
```json
{
  "message": "Book deleted successfully"
}
```

## Running Locally
To run this API locally:

1. Clone the repository:
   ```sh
   git clone <your-repo-url>
   cd <your-repo-folder>
   ```

2. Install dependencies:
   ```sh
   go mod tidy
   ```

3. Start the server:
   ```sh
   go run main.go
   ```

## Tech Stack
- **Golang**
- **MongoDB (Atlas)**
- **Gorilla Mux**
- **Railway for Deployment**

## Contact
If you have any questions or need help, feel free to ask!

