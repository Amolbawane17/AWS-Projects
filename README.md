# AWS-Projects
Creating an project with Various AWS service like aws lambda, dyanamoDB, API gateways, CLoudtrail etc,

Steps to be followed:
Create role in IAM for lambda, keep admin access for s3, dynamodb, api integration for smooth process
  First stored required file in s3 bucket in .zip format
  create function in lambda, upload file from s3 bucket (don't perform testing)
  create table in dynamoDB
  now, For API integration, select REST API build, keep api endpoint regional, security policy(keep recommended) and tap create API.
  Now we have to create two method (GET, POST)
     Select Crete method option , 
     mehtod type - GET,
     Integration type - Lambda Function, 
     then enable to lambda proxy integration
     Choose region and ARN of your lambda function, then hit create method button
     DO THE SAME FOR POST METHOD
     After this, you need to depoly your API, go to deploy API option, choose **new stage** option and provide name (dev or prod) and submit
     now copy invoke URL(it would be your link for website) and saved it in your notepad

  Now run your deploy and test your lambda function. Done
     
