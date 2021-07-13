# Sentiment Analysis on AWS Tutorial

### Agenda
0. [Data Source Configuration](docs/DataSource.md)
1. [Sentiment Analysis on AI Services](docs/AIServices.md)
2. [Data Labelling using SageMaker Ground Truth](docs/DataLabelling.md)
3. [Data Engineering, Training, and Deployment using SageMaker](docs/DevelopmentSM.md)

### Scope of Project
1. Sentiment Analysis is using Supervised Approach text classification using BlazingText on SageMaker (More description for [BlazingText is Here](https://docs.aws.amazon.com/sagemaker/latest/dg/blazingtext.html)).
2. Sentiment Analysis is using Indonesian Twitter Dataset [here](http://ridi.staff.ugm.ac.id/2019/03/06/indonesia-sentiment-analysis-dataset/)
3. For data labelling, it will only use 10 tweets, to short the amount of time.
4. Since Indonesian language is not supported on NLP AI service on AWS, we need to translate it to english to be consumed to NLP Service (Comprehend).