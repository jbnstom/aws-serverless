# aws-serverless
Simple serverless application using AWS

Install Serverless

Open your console and type (put sudo before if you are using Linux)

$ npm install -g serverless

Configure AWS IAM keys

$ serverless config credentials --provider aws --key xxxxxxxxxxxxxx --secret xxxxxxxxxxxxxx

keys can be obtained from My Security Credentials in the AWS Console.

Create a simple project

$ serverless create --template aws-nodejs --path serverless-aws-nodejs

Serverless created a new folder with inside a basic NodeJS service. The principal files are:

    serverless.yml: it’s the main config file of Serverless
    handlers.js: it does contain the NodeJS application
    
To Deploy

$ serverless deploy
