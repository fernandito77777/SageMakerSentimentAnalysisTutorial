# Sentiment Analysis Tutorial

### Agenda
1. [Data Labelling using SageMaker Ground Truth](docs/DataLabelling.md)
2. [Data Engineering, Training, and Deployment using SageMaker](docs/DevelopmentSM.md)
3. [Sentiment Analysis on AI Services](docs/AIServices.md)

### Data Source
1. Please download this [Indonesian Tweet dataset](files/SentimentAnalysis-IndonesiaData.zip). Unzip it once you are done.
2. Alternatively, if you can't unzip files, here is the [data for label](../files/IndonesianTweetUnlabelled.csv) and [data for ML Process](files/IndonesianTweetlabeled.csv)

### Scope of Project
1. Sentiment Analysis is using Supervised Approach text classification using BlazingText on SageMaker.
2. Sentiment Analysis is using Indonesian Twitter Dataset [here](http://ridi.staff.ugm.ac.id/2019/03/06/indonesia-sentiment-analysis-dataset/)
3. For data labelling, it will only use 10 tweets, to short the amount of time.
4. Since Indonesian language is not supported on NLP AI service on AWS, we need to translate it to english to be consumed to NLP Service (Comprehend).