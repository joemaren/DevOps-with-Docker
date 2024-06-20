# Exercise 1.14: Environment
# Create a Dockerfile to run the backend of the project, set the environment
# variable to allow cross-origin resource sharing (CORS) request from the 
# frontend.

FROM golang:latest

ENV PORT=8080

EXPOSE 8080

ENV REQUEST_ORIGIN="http://localhost:5000"

WORKDIR /usr/src/app

COPY . .

RUN go build

CMD ./server
