# Session 09 - Exercise 3

## HTML
<h1>Hello Docker Session 09!</h1>

## Dockerfile
FROM nginx:alpine
COPY index.html /usr/share/nginx/html/index.html

## Build
docker build -t my-html-app:v1 .

## Run
docker run -d -p 8081:80 --name html-app my-html-app:v1

## Test
curl.exe http://localhost:8081

## Expected result
<h1>Hello Docker Session 09!</h1>