# Go CRUD App with Gorilla Mux
This is a simple CRUD (Create, Read, Update, Delete) web application built with Go and the Gorilla Mux router. The application allows you to perform CRUD operations on a collection of movie data, including the movie's ID, ISBN, title, and director information.
## Requirements
* [Go](https://go.dev/dl/) (version 1.16 or higher)
* [Gorilla Mux](https://github.com/gorilla/mux) (version 1.8.0 or higher)
## Installation and Setup
1. Clone the repository: `git clone https://github.com/Supsource/Golang-Projects/tree/main/CRUD-Movies-App`
2. Navigate to the project directory: `cd CRUD-Movies-App`
3. Install the Gorilla Mux router: `go get -u github.com/gorilla/mux`
4. Run the application: `go run main.go`
5. Open your web browser and go to `http://localhost:8000`
## Usage
The following endpoints are available:
* `GET /movies`: retrieves all movies
* `GET /movies/{id}`: retrieves a single movie by ID
* `POST /movies`: creates a new movie
* `PUT /movies/{id}`: updates an existing movie by ID
* `DELETE /movies/{id}`: deletes a movie by ID
## Example Request and Response
Create a new movie:

* Request:
```json
{
  "isbn": "0123456789",
  "title": "My Movie",
  "director": {
    "firstname": "John",
    "lastname": "Doe"
  }
}
```
* Response:
```json
{
  "id": "1234567",
  "isbn": "0123456789",
  "title": "My Movie",
  "director": {
    "firstname": "John",
    "lastname": "Doe"
  }
}
```
