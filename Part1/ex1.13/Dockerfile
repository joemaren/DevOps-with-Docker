# Exercise 1.13: HELLO, BACKEND!
# Create a Dockerfile for the project (example-backend).

FROM golang:latest

ENV PORT=8080

EXPOSE 8080

WORKDIR /usr/src/app

# build the go application
RUN go build

# run the webserver
CMD ./server


