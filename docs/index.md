# PDF Render Service

Generate beautiful PDFs from HTML templates using .NET 8, Handlebars and Playwright.

---

## What this service does

Convert HTML templates into PDF documents using JSON data.

Perfect for:

• invoices
• reports
• certificates
• statements
• agreements

---

## How it works

1. Send HTML template
2. Send JSON data
3. API merges template
4. Playwright renders PDF

---

## Quick Start

Run container:

docker run -p 8080:80 websvcin/pdf-service

Swagger UI:

http://localhost:8080/docs

---

## Example Output

Professional invoice generated using template:

![invoice](assets/invoice-preview.png)

---

## Preview Example

Live template preview:

https://websvcin.github.io/pdf-service/assets/invoice-preview.html

## Links

Docker Hub:
https://hub.docker.com/r/websvcin/pdf-service

GitHub:
https://github.com/websvcin/pdf-service

---
