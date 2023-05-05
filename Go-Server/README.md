# Simple Go Server
This is a simple web server written in Go that serves static files and handles HTTP requests for form data and a simple greeting.
## Prerequisites
To run this server, you'll need to have Go installed on your system. You can download and install the latest version of Go from the official [Go website](https://go.dev/).
## Getting Started
To get started, clone this repository to your local machine:
```
$ git clone https://github.com/Supsource/Golang-Projects
```
Once you have the repository cloned, navigate to the project directory:
```
$ cd go-server
```
Next, run the following command to start the server:
```
$ go run main.go
```
You should see the following message in your terminal:
```
Starting the server at port 8080
```
This means that the server is now running and listening for requests on port 8080.

## Usage
Once the server is running, you can access it by opening a web browser and navigating to `http://localhost:8080`. This will display the index.html file in the "static" directory.


To access the form handler, navigate to `http://localhost:8080/form`. This will display a form where you can enter your name and address. Submitting the form will display the values of the "name" and "address" fields.


To access the hello handler, navigate to `http://localhost:8080/hello`
