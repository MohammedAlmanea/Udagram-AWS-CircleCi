# Hosting a Full-Stack Application

[![MohammedAlmanea](https://circleci.com/gh/MohammedAlmanea/Udagram-AWS-CircleCi.svg?style=svg)](https://app.circleci.com/pipelines/github/MohammedAlmanea/Udagram-AWS-CircleCi)

## Udagram Overview

Udagram - an Image Filtering application, allows users to register and log into a web client, post photos to the feed, and process photos using an image filtering service. It has two components:

- Frontend - Angular web application built with Ionic framework.
- Backend RESTful API - Node-Typescript application.

## Diagrams

### Architecture

![Architecture Diagram](./diagrams/AWS-Architecture.png)

### Pipeline

![Pipeline Diagram](./diagrams/Pipeline-Diagram.png)

## Project URLS

API : http://udagram-api-dev.eba-wgsa4svp.us-east-1.elasticbeanstalk.com  
Front-End : http://mohammed-udagram.s3-website-us-east-1.amazonaws.com

### Installation

Provision the necessary AWS services needed for running the application:

1. In AWS, provision a publicly available RDS database running Postgres. <Place holder for link to classroom article>
1. In AWS, provision a s3 bucket for hosting the uploaded files. <Place holder for tlink to classroom article>
1. Export the ENV variables needed or use a package like [dotnev](https://www.npmjs.com/package/dotenv)/.
1. From the root of the repo, navigate udagram-api folder `cd starter/udagram-api` to install the node_modules `npm install`. After installation is done start the api in dev mode with `npm run dev`.
1. Without closing the terminal in step 1, navigate to the udagram-frontend `cd starter/udagram-frontend` to intall the node_modules `npm install`. After installation is done start the api in dev mode with `npm run start`.

## Testing

This project contains two different test suite: unit tests and End-To-End tests(e2e). Follow these steps to run the tests.

1. `cd starter/udagram-frontend`
1. `npm run test`
1. `npm run e2e`

There are no Unit test on the back-end

### Unit Tests:

Unit tests are using the Jasmine Framework.

### End to End Tests:

The e2e tests are using Protractor and Jasmine.

## Built With

- [Angular](https://angular.io/) - Single Page Application Framework
- [Node](https://nodejs.org) - Javascript Runtime
- [Express](https://expressjs.com/) - Javascript API Framework
