# Udagram

This application is provided by Udacity in the Fullstack Javascript program as a base project for the 'Hosting a Full-Stack Application' assigment. The udagram application is a fairly simple application that includes all the major components of a Full-Stack web application.


## Getting Started

1. Clone this repo locally into the location of your choice.

Each project (udagram-api and udagram-frontend) can be installed and run, but they need some information to connect to the database and storage service.

### Dependencies

```
- Node v14.15.1 (LTS) or more recent. While older versions can work it is advisable to keep node to latest LTS version

- npm 6.14.8 (LTS) or more recent, Yarn can work but was not tested for this project

- AWS CLI v2, v1 can work but was not tested for this project

- A RDS database running Postgres.

- A S3 bucket for hosting uploaded pictures.

```

### Local Installation

Provision the necessary AWS services needed for running the application:

1. In AWS, provision a publicly available RDS database running Postgres. <Place holder for link to classroom article>
1. In AWS, provision a s3 bucket for hosting the uploaded files. <Place holder for tlink to classroom article>
1. Export the ENV variables needed or use a package like [dotnev](https://www.npmjs.com/package/dotenv)/.
1. From the root of the repo, navigate udagram-api folder `cd starter/udagram-api` to install the node_modules `npm install`. After installation is done start the api in dev mode with `npm run dev`.
1. Without closing the terminal in step 1, navigate to the udagram-frontend `cd starter/udagram-frontend` to install the node_modules `npm install`. After installation is done start the api in dev mode with `npm run start`.


## Hosting Assigment
The `docs` folder includes:
- A screenshot of last build in CircleCi
- A screenshot of configured database AWS RDS
- A screenshot of configured AWS S3
- A screenshot of configured AWS Elastic Beanstalk General view
- A screenshot of configured CircleCI Environment variables
- A 'Hosted Fullstack Application' diagram
- A 'Pipeline Overview' diagram
- An App Dependencies document
- An Infrastructure Description document
- A Pipeline Process document

The link to the hosted EB api:
[http://udagramapinode12-env.eba-pbjyxrkj.us-east-1.elasticbeanstalk.com/](http://udagramapinode12-env.eba-pbjyxrkj.us-east-1.elasticbeanstalk.com/)

The link to the hosted Front-End Application is:
[http://udagram-ew.s3-website-us-east-1.amazonaws.com/](http://udagram-ew.s3-website-us-east-1.amazonaws.com/)

### Project's build badge
[![esteban-w](https://circleci.com/gh/esteban-w/udagram.svg?style=svg)](https://app.circleci.com/pipelines/github/esteban-w/udagram)

### Checking FE app functionality
To test data storing and retrieving is functioning:
1. Navigate to  [http://udagram-ew.s3-website-us-east-1.amazonaws.com/](http://udagram-ew.s3-website-us-east-1.amazonaws.com/)
2. Register clicking the 'register' button, provide name, email, password
3. Log out and log in to test functionality


### Testing applications

This project contains two different scripts to run tests:
- for Backend API application (pending to be added), from root folder run:
  `npm run backend:tests`
- for Frontend application (unit tests and End-To-End tests), from root folder run:
  `npm run frontend:tests`


### Frontend Unit Tests:

Unit tests are using the Jasmine Framework.

### Frontend End to End Tests:

The e2e tests are using Protractor and Jasmine.

## Built With

- [Angular](https://angular.io/) - Single Page Application Framework
- [Node](https://nodejs.org) - Javascript Runtime
- [Express](https://expressjs.com/) - Javascript API Framework

## License

[License](LICENSE.txt)
