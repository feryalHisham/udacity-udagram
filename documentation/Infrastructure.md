# Project Infrastructure

This project consists of 3 parts: frontend, backend APIs and database.

1. Frontend: Angular application where the entry file is the index.html. The frontend is built and uploaded to AWS S3 bucket. User can see the rendered html pages and iteract with them through a link opened in a browser.
2. Backend: APIs built with Nodejs and Express. Frontend call APIs through HTTP requests and recieves a response. Backend is deployed on AWS Elastic Beanstalk.
3. Database: Postgres database to save users and feeds. The database is hosted on AWS RDS. Backend performs CRUD operations on the database
