# AWS Lambda layers for Python Git

This project provides the requisite files to make git commands in Python in AWS Lambdas. Lambda functions don't natively have git installed, so two files are required: 
* one file to install the git binary
* one file to install the required GitPython modules (see https://pypi.org/project/GitPython/)

1. Install these two zip files as layers in AWS Lambda. 
2. Then import the layers into your lambda function
