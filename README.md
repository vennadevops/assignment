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









