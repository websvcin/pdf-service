# PDF Render Service

Generate PDFs from HTML templates using .NET 8, Handlebars, and Playwright.

---

## Quick Start

Run docker:

docker run -p 8080:80 websvcin/pdf-service

Swagger UI:

http://localhost:8080/docs

---

## API Endpoint

POST /api/render/pdf

---

## Example

HTML:

<h1>Hello {{name}}</h1>

JSON:

{
"name":"John"
}

---

## Links

Docker Hub:
https://hub.docker.com/r/websvcin/pdf-service

GitHub:
https://github.com/websvcin/pdf-service
