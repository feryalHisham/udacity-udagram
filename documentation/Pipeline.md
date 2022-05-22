# Pipeline Process

The pipeline process is the process of building and deploying both the frontend and backend automatically. It is managed by circleci integrated with github.

Before running the pipeline we need first to setup the project by linking circleci project to the required repo and repo branch.

The pipeline consists of the following steps:

1. Set up the docker container where the pipeline jobs will run.
2. Install Nodejs and aws cli.
3. Checkout to get the latest code.
4. Install Client-Side(Frontend) Dependency Packages
5. Build Client-Side
6. Install Server-Side(Backend) Dependency Packages
7. Build Server-Side
8. Upload Client-Side build to S3 bucket
9. Deploy Server-side build on Elastic Beanstalk
