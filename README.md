To achieve this assignment followed below steps.

1. created ec2 instance with ubuntu operating system.

![image](https://user-images.githubusercontent.com/56083714/66061561-53133e00-e55d-11e9-9674-5ded0aaaa1f4.png)

2. Dockerizing node js application
In the first part of this guide we will create a simple web application in Node.js, then we will build a Docker image for that application.

Create the Node.js app

First, create a new directory where all the files would live. In this directory create a package.json file that describes your app and its dependencies:

![image](https://user-images.githubusercontent.com/56083714/66062207-99b56800-e55e-11e9-92e2-2ca35e14148f.png)

With your new package.json file, run npm install. If you are using npm version 5 or later, this will generate a package-lock.json file which will be copied to your Docker image.

Then, create a server.js file that defines a web app using the Express.js framework:

![image](https://user-images.githubusercontent.com/56083714/66062473-1f391800-e55f-11e9-9cf1-1f8831f38577.png)

In the next steps, we'll look at how you can run this app inside a Docker container using the official Docker image. First, you'll need to build a Docker image of your app.

Creating a Dockerfile

![image](https://user-images.githubusercontent.com/56083714/66062769-aab2a900-e55f-11e9-8289-1231585cf47f.png)

.dockerignore file

Create a .dockerignore file in the same directory as your Dockerfile with following content:

node_modules
npm-debug.log

This will prevent your local modules and debug logs from being copied onto your Docker image and possibly overwriting modules installed within your image.

now pulling the mongo db image and building node.js docker file using docker compose file.

docker-compose up -d


![image](https://user-images.githubusercontent.com/56083714/66063333-c5395200-e560-11e9-8911-98e5af12ffe6.png)

After running docker-compose up -d command then we can see containers are running like below.

![image](https://user-images.githubusercontent.com/56083714/66064229-a2a83880-e562-11e9-80ce-0f10cea19ad7.png)


and then folder structure should be like below.

![image](https://user-images.githubusercontent.com/56083714/66063586-4d1f5c00-e561-11e9-9b23-2cea9ddf4f4a.png)

now mongo DB and application both containers are running and lets connect to both containers.




















