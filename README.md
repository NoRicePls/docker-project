# docker-project

# Hello World Docker Container

pushed to [Docker Hub
](https://hub.docker.com/r/u1ih/hello)

Run with:

`docker run -d -p 8080:8080 u1ih/hello`

Steps:

## 1: Get Source

`git clone https://github.com/u1i/docker-hello`

## 2: Make changes

modify index.html in the app directory

## 3: Build Container

`docker build .`  (take note of the new IMAGE_ID)

## 4: Tag Container and push to Dockerhub

`docker tag <IMAGE_ID> <YOUR_USERNAME>/hello:<VERSION_NUMBER>`

`docker tag <IMAGE_ID> <YOUR_USERNAME>/hello:latest`

`docker login`

`docker push <YOUR_USERNAME>/hello:<VERSION_NUMBER>`

`docker push <YOUR_USERNAME>/hello:latest`

## 5: Run Container

`docker run -d -p 8080:8080 <YOUR_USERNAME>/hello`
