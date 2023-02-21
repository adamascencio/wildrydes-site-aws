# Building a Serverless Web Application on AWS

This tutorial from AWS teaches how to build a serverless web application on AWS using a combination of services such as AWS Lambda, Amazon API Gateway, Amazon S3, Amazon DynamoDB, and Amazon Cognito. 

By following the tutorial, I'll learn how to create a web application that allows users to register, log in, and upload images. The tutorial also covers how to store the images in Amazon S3, how to use Amazon DynamoDB to store user data, and how to secure your application with Amazon Cognito.

The tutorial is divided into several modules, and each module covers a specific aspect of building the web application. The modules include:

- Setting up the AWS environment
- Creating the AWS Lambda function
- Creating the Amazon API Gateway
- Creating the Amazon S3 bucket
- Creating the Amazon DynamoDB table
- Creating the Amazon Cognito user pool and identity pool
- Building the web application

At the end of the tutorial, I'll have a fully functional web application that is deployed on AWS and can be accessed via the internet. 

To access the deployed site for this tutorial, [click here](https://main.dyisqfmjcmbf8.amplifyapp.com/).
To view the AWS tutorial for this project, [click here](https://aws.amazon.com/getting-started/hands-on/build-serverless-web-app-lambda-apigateway-s3-dynamodb-cognito/).

## Challenges
#### Outdated Tutorial
The tutorial provided in this repository was not up to date with the current version of ArcGIS. I encountered issues when attempting to sign in to ArcGis which renders the application's map. I found on StackOverflow that this was a common issue and just required updating the script from version 4.3 to 4.6. I updated the script and the map now renders properly.

#### JS Starter Code Not Working as Expected
In the starter code, there is a JS function that is supposed to convert the user's email input to a username when creating a user in AWS' Cognito User Pool. The function removed the email's @ symbol and replaced it with "-at-". This invalidated the email address and the user was not able to register.

To address this issue, I reviewed the register page's script and found the function which generated a username for AWS Cognitio. I removed the replace method which invalidated the user's email, and that fixed the issue.

## Finished Product
[images/map.png]