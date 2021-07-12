## Sentiment Analysis on AI Services

for AI Services, we are going to use Comprehend, NLP Service on AWS. Currently, there are only limited [supported languages on Comprehend here](https://docs.aws.amazon.com/comprehend/latest/dg/supported-languages.html). But, that doesn't mean we can't use it. There are several ways to do it, and one of them is to translate the content from other language to English.

On this workshop since we have used Indonesian language, we will use pre-translated data from previous workshop (Indonesian to English language). It has been translated using Amazon Translate, by following [this approaches](https://aws.amazon.com/blogs/machine-learning/translating-documents-with-amazon-translate-aws-lambda-and-the-new-batch-translate-api/)

This step is following [this AWS Blog](https://aws.amazon.com/blogs/machine-learning/active-learning-workflow-for-amazon-comprehend-custom-classification-part-1/)

1. go to [this link](https://console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacks/create/template?templateURL=https://aws-ml-blog.s3.amazonaws.com/artifacts/create-retraining-workflow-for-custom-classification-models-in-Amazon-Comprehend/cft1/templateS3.yaml). It will open CloudFormation page.

CloudFormation is a service that runs the infrastructure based on code. it will create a template of infrastructure (on YAML, or JSON file) that is useful for scalability and reusability of the infrastructure.

2. 


[BACK TO WORKSHOP GUIDE :house:](../README.md)

[BACK TO PREVIOUS GUIDE :arrow_left:](DevelopmentSM.md)