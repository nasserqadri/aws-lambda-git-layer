# AWS Lambda layers for Python Git

This project provides the requisite files to make git commands in Python in AWS Lambdas. Lambda functions don't natively have git installed, so two files are required: 
* one file to install the git binary
* one file to install the required GitPython modules (see https://pypi.org/project/GitPython/)

I tried to use the ARNs provided here, but they didn't work for my instance: https://github.com/lambci/git-lambda-layer 

For now I've just provided the two zip files. In the future, I'll include notes on how to create these in case users want to ingest a different version of either the modules or the git binary.

## Installation instructions
1. Install these two zip files as layers in AWS Lambda. 
2. Then import the layers into your lambda function
