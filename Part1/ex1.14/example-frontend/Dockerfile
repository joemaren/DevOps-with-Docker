# Exercise 1.14: ENVIRONMENT
# Create a Dockerfile to run the frontend for the project with the correct
# ports exposed and the environment varaiable for the backend set.
FROM node:16.20.2

EXPOSE 5000

WORKDIR /usr/src/app

COPY . .

ENV REACT_APP_BACKEND_URL=http://127.0.0.1:8080

RUN npm install
 
RUN npm run build

RUN npm install -g serve

CMD serve -s -l 5000 build
