# Full Example

## Step 1 HTML template

<h1>Hello {{name}}</h1>

---

## Step 2 convert to base64

node example:

const html = "<h1>Hello {{name}}</h1>"

Buffer.from(html).toString("base64")

---

## Step 3 call API

curl:

curl -X POST http://localhost:8080/api/render/pdf 
-H "Content-Type: application/json" 
-d '{
"template":{
"type":"base64",
"content":"PGgxPkhlbGxvIHt7bmFtZX19PC9oMT4="
},

"data":{
"name":"John"
}

}'

---

## Step 4 decode pdf

const pdf = atob(response.pdfBase64)

---

## result

PDF file generated

---
