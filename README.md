# this is a template for build an ML-Batch-Pipeline

## Included AWS Services

* Cloudwatch
* Lambda
* Batch ec2
* SNS
* SQS

## Idea

The idea is to create a cloudwatch alarm, which will be triggered when there are messages sent to a SQS-Queue. This alarm publishes a Message to a SNS-Topic, which will trigger a lambda-function. The lambda function, will start based on the sqs length an AWS Batch Job Array.  
