# Getting Started

## Step 1 pull docker image

docker pull websvcin/pdf-service

---

## Step 2 run container

docker run -p 8080:80 websvcin/pdf-service

---

## Step 3 open swagger

http://localhost:8080/docs

---

## Step 4 test endpoint

POST

/api/render/pdf

---

## Request example

{
"template":{
"type":"base64",
"content":"BASE64_HTML"
},

"data":{
"name":"John"
}
}

---
