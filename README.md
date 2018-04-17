# React / Docker multi-stage setup 

Example on how to deploy a create-react-app into production with docker multi-stage build. This project uses NGINX as webserver.

Build the Docker image:
```
docker build -t example/myapp .
```

Run your application-container with:
```
docker run -d -p 8080:80 example/myapp
```

And access using [http://localhost:8080](http://localhost:8080)

The React project has been initialized with [create-react-app](https://github.com/facebook/create-react-app) by Facebook
