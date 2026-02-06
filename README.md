# Go REST API – Dockerized

A minimal **Go (Golang) REST API** containerized with Docker using multi‑stage builds and Alpine runtime.  
It exposes a simple JSON endpoint.

---

## Project Structure
docker-go-demo/
├── Dockerfile
├── main.go
├── .dockerignore
└── README.md

---

## Application Overview
- **Language:** Go  
- **Port:** 8080  
- **Endpoint:** `/`  
- **Response:**
  ```json
  { "message": "Hello from Go + Docker!" }
Run Locally


go run main.go
# open http://localhost:8080

Run with Docker

Build Image

docker build -t rahulrokksss/golang:0.0.1.RELEASE .

Run Container

docker run -d -p 8080:8080 rahulrokksss/golang:0.0.1.
RELEASE

Access

Open http://localhost:8080

Author

Rahul Shukla