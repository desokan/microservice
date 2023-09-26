# Blog Microservices

## Project Description

Blog microservices project with Node JS, React and MongoDB. The services will run with Docker and I will be using Kubernetes for orchestrating the different services. I will also be leveraging Google Cloud environment for the development. Finally, I will use GitHub Actions for CI/CD.

The project is designed using microservices and it comprises of a react client for the froentend, posts service, comments service, event bus and query service. Each one is a separate project. To run the project, follow the steps below.

## React Client

Install the dependencies defined inside the package.json file.

`npm install`

To start the react app, run the following command in the terminal:

`npm start`

## Posts Service

Install the dependencies defined inside the package.json file.

`npm install`

To start the posts service, run the following command in the terminal:

`npm start`

This service is running on port 4000.

## Comments Service

Install the dependencies defined inside the package.json file.

`npm install`

To start the comments service, run the following command in the terminal:

`npm start`

This service is running on port 4001.

## Query Service

Install the dependencies defined inside the package.json file.

`npm install`

To start the query service, run the following command in the terminal:

`npm start`

This service is running on port 4002.

## Event Bus

Install the dependencies defined inside the package.json file.

`npm install`

To start the event bus service, run the following command in the terminal:

`npm start`

This service is running on port 4005.

## Testing the project

Fill the posts form on the homepage. This will create a new post. At this point, observe the `event-bus` terminal running on port 4005 and see the output of the event emitted.

Similarly, add a comment to the post using the comment form attached to the post. This post request hits the endpoint defined in the `posts service`, which then emits an event to the `event-bus`. Check the terminals for the outputs.