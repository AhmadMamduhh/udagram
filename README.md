
# Udagram Full-Stack Application


 The Udagram application is a fairly simple application that includes all the major components of a Full-Stack web application. This repo contains a full Node.js API as backend, an Angular project as a frontend & a CircleCi pipeline config file to handle installing packages, linting, building & deploying for both the frontend and the backend. The frontend is hosted on an AWS S3 bucket and the backend API is hosted on an AWS Elastic Beanstalk server. The backend is connected to a Postgres database which is hosted on AWS RDS.

### Web App Screenshots
The web app is hosted on an AWS S3 bucket. Here's the link to access it: http://udagram-web.s3-website-us-east-1.amazonaws.com/home

 1. Home Page
https://drive.google.com/file/d/1KTFRoyS2yY1t06u8aINXB7PbC1wW9MGO/view?usp=sharing

 2. Registration Dialog
 https://drive.google.com/file/d/1hQ11PBk213bs3b9XmP97fo7ggS-WmQum/view?usp=sharing

 3. Logged In Home Page
 https://drive.google.com/file/d/1OYzM1imVjGTvT1aYIELMMo3TUOp2VyfB/view?usp=sharing

 4. Post Photo Dialog
 https://drive.google.com/file/d/16Wm-6W40Pac-0apIwqMpR2iyHDUDBYXL/view?usp=sharing

  

### Dependencies

  

```

- Node v14.15.1 (LTS) or more recent. While older versions can work it is advisable to keep node to latest LTS version

  

- npm 6.14.8 (LTS) or more recent, Yarn can work but was not tested for this project

  

- AWS CLI v2, v1 can work but was not tested for this project

  

- A RDS database running Postgres.

  

- A S3 bucket for hosting uploaded pictures.

  

```

  

### Installation


Provision the necessary AWS services needed for running the application:


1. In AWS, provision a publicly available RDS database running Postgres. Here's the hostname of the Postgres database: udagram-db.cym3wyagliht.us-east-1.rds.amazonaws.com

2. In AWS, provision a S3 bucket for hosting frontend Angular web app. Here's the link of the Angular web app deployed on S3: http://udagram-web.s3-website-us-east-1.amazonaws.com

3. Export the ENV variables needed or use a package like [dotnev](https://www.npmjs.com/package/dotenv).

4. From the root of the repo, navigate udagram-api folder `cd udagram/udagram-api` to install the node_modules `npm install`. After installation is done start the api in dev mode with `npm run dev`.

5. Without closing the terminal in step 1, navigate to the udagram-frontend `cd udagram/udagram-frontend` to install the node_modules `npm install`. After installation is done start the api in dev mode with `npm run start`.

  

## Testing

  

This project contains two different test suite: unit tests and End-To-End tests(e2e). Follow these steps to run the tests.

  

1.  `cd starter/udagram-frontend`

1.  `npm run test`

1.  `npm run e2e`

  

There are no Unit test on the back-end

  

### Unit Tests:

  

Unit tests are using the Jasmine Framework.

  

### End to End Tests:

  

The e2e tests are using Protractor and Jasmine.

  

## Built With

  

- [Angular](https://angular.io/) - Single Page Application Framework

- [Node](https://nodejs.org) - Javascript Runtime

- [Express](https://expressjs.com/) - Javascript API Framework

-  [AWS](https://aws.amazon.com/?nc2=h_lg) - Cloud Services Provider

  

## License

  

[License](LICENSE.txt)