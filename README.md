# Getting Started with Docker

Go Hello World
---
This is a simple Go web application that prints a "Hello World" message.

Run the application
---
This application listens on port `6111`

To run the application, use the following command:
```
go run main.go 
```
Access the application on: http://127.0.0.1:6111/

Steps to package the application using Docker commands:
---
``` 
# build the image
docker build -t go-helloworld .

# run the image
docker run -d -p 6111:6111 go-helloworld

# tag the image
docker tag go-helloworld pixelpotato/go-helloworld:v1.0.0

# push the image
docker push pixelpotato/go-helloworld:v1.0.0

# login into DockerHub
docker login
```

