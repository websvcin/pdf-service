# API Reference

## POST /api/render/pdf

Generates PDF from HTML template.

---

## request body

RenderRequest

template.content

base64 encoded html

---

data

json object

---

options

pageSize:

A4
Letter

orientation:

portrait
landscape

---

## response

pdfBase64

base64 encoded pdf

---

## CURL example

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
