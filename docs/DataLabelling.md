## Data Labelling using SageMaker Ground Truth

SageMaker Ground Truth is a segment on SageMaker, ML Platform on AWS that helps to label the data you would like to process on Machine Learning. For more description, please click [here](https://docs.aws.amazon.com/sagemaker/latest/dg/sms.html)

1. Please download this [Indonesian Tweet dataset](../files/SentimentAnalysis-IndonesiaData.zip). Unzip it once you are done.
2. Alternatively, if you can't unzip files, here is the [data for label](../files/IndonesianTweetUnlabelled.csv) and [data for ML Process](../files/IndonesianTweetlabeled.csv)
3. Go to [AWS Console](https://ap-southeast-1.console.aws.amazon.com/console/home?region=ap-southeast-1#)
4. type `SageMaker` at the search bar
5. click `Ground Truth` menu at the right side.
6. click `Labeling workforces` at the submenu.
7. click `Private` tab.

There are 3 ways to label your data on SageMaker Ground Truth:
* Mechanical Turk
    On-demand workers that can help to label the data. there is a human that will label your own data, given your description on how to label your data.
* Private
    Your own team will label the data, by creating private team for label and assign it to individuals by email.
* Vendor
    3rd party vendor that will help you to label your data. by using AWS Marketplace, you will be able to ask for their service.

For current workshop, we're going to use Private way.

8. on Private tab, click `Create private team`
9. in create private team page, choose `Create a private team with AWS Cognito`

AWS Cognito is a service that helps for authentication and authorization for users in a system. In this case, since there will be users who are going to label the data, they require authroization to label it.

10. Fill the team name with `LabelerTeam`
11. in add workers, choose `invite new workers by email`
12. fill your email address
13. fill the organization name and contact email. for contact email, you can fill your own email again.
14. click `Create private team`
15. in your private team, click your team name (`LabelerTeam`)
16. click `Workers` tab
17. Make sure your email is there.

You will receive an email invitation to label the data. Open it later.

Now, we are going to upload our data that will be labelled.

---
move to data source step
---

Once it's done, let's go back to Ground Truth to set the label job.

27. go to [SageMaker Console](https://ap-southeast-1.console.aws.amazon.com/sagemaker/home?region=ap-southeast-1#/landing)
28. click `Ground Truth` menu at the left side and click `Labeling Job`
29. click `Create labelling job`
30. in job overview page, fill the job name with `SentimentAnalysisIndoJobLabel`
31. in input data setup, choose `Automated data setup`
32. click `Browse S3` button
33. choose your bucket, and click `Choose`
34. in data type, click `Text`
35. in IAM Role, click the dropdown and click `Create a new role`
36. in S3 bucket, click `Any S3 bucket`
37. click `Create`

it will create a role for us to access the data from S3.

38. click `Complete data setup` button

this will create a manifest file, acts as a pointer that the data will be used to labe

[BACK TO WORKSHOP GUIDE :house:](../README.md)

[CONTINUE TO NEXT GUIDE :arrow_right:](DevelopmentSM.md)