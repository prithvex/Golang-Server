# Go HTTP Web Server

A simple web server built with **Go (Golang)** using the standard `net/http` package. This project demonstrates how to serve static web pages, handle routes, and process HTML form submissions.

## Features

* 🚀 Serve static HTML pages
* 📄 Home page (`index.html`)
* 📝 Contact form (`form.html`)
* 📬 Handle form submissions using POST requests
* 👋 Simple `/hello` endpoint
* ⚡ Built entirely with Go's standard library (`net/http`)

## Project Structure

```text
go-http-server/
│── main.go
│── README.md
│
└── static/
    ├── index.html
    └── form.html
```

## Prerequisites

* Go 1.20 or later

Check your Go installation:

```bash
go version
```

## Running the Project

Clone the repository:

```bash
git clone https://github.com/<your-username>/<repository-name>.git
```

Move into the project directory:

```bash
cd <repository-name>
```

Run the application:

```bash
go run main.go
```

The server will start on:

```text
http://localhost:8000
```

## Available Routes

| Route        | Method | Description                      |
| ------------ | ------ | -------------------------------- |
| `/`          | GET    | Serves `index.html`              |
| `/form.html` | GET    | Displays the HTML form           |
| `/form`      | POST   | Receives and processes form data |
| `/hello`     | GET    | Returns `Hello!`                 |

## Form Submission

The form sends a POST request to:

```text
/form
```

Example fields:

* **Name**
* **Address**

Example response:

```text
POST Request Successful
Name = John
Address = New York
```

## Technologies Used

* Go (Golang)
* net/http
* HTML5

## Learning Objectives

This project helps beginners understand:

* Creating an HTTP server in Go
* Serving static files
* Routing requests
* Handling GET and POST methods
* Processing HTML forms
* Reading user input with `FormValue()`
* Sending responses using `http.ResponseWriter`

## Future Improvements

* Add CSS styling
* Use HTML templates
* Store form data in a database
* Add JavaScript validation
* Build a REST API
* User authentication
* Session management

## License

This project is open source and available under the MIT License.
