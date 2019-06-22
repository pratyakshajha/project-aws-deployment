## Project Overview

This repository hosts code used in fifth project on deploying Neural Networks project in the Deep Learning Nanodegree. 

Given a review of a moview, the algorithm will classofy its sentiments as either positive or negative.
## Project To Do List

### Rubrics
| Criteria                                           | Specifications                                                                                                                                                                                        | Finished |
|----------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------|
| Submission Files                     | The submission includes all required files, including notebook, python scripts and html files.            |<ul><li>[x] </li></ul>|
| What does review_to_words do?                           | Answer describes what the pre-processing method does to a review. |<ul><li>[x] </li></ul>|
| Create a word dictionary                            | The build_dict method is implemented and constructs a valid word dictionary.      |<ul><li>[x] </li></ul>|
| What are the five most frequently appearing words? | Notebook displays the five most frequently appearing words.   |<ul><li>[x] </li></ul>|
| Understanding `preprocess_data` and `convert_and_pad_data`               | Answer describes how the processing methods are applied to the training and test data sets and what, if any, issues there may be.  |<ul><li>[x] </li></ul>|
| Writing the training method               | The train method is implemented and can be used to train the PyTorch model. |<ul><li>[x] </li></ul>|
| Training the model               | The RNN is trained using SageMaker's supported PyTorch functionality.   |<ul><li>[x] </li></ul>|
| Deploy the trained model             | The trained PyTorch model is successfully deployed.  |<ul><li>[x] </li></ul>|
| How does this model compare to the XGBoost model?               | Answer describes the differences between the RNN model and the XGBoost model and how they perform on the IMDB data. |<ul><li>[x] </li></ul>|
| Process the test review               | The test review has been processed correctly and stored in the test_data variable.  |<ul><li>[x] </li></ul>|
| Writing inference code               | The `predict_fn()` method in serve/predict.py has been implemented.  |<ul><li>[x] </li></ul>|
| The web app is deployed               | The model is deployed and the Lambda / API Gateway integration is complete so that the web app works (make sure to include your modified index.html). |<ul><li>[x] </li></ul>|
| Give an example review and response               | Answer gives a sample review and the resulting predicted sentiment.  |<ul><li>[x] </li></ul>|
| Prepare report                        | Refer the [rubrics](https://review.udacity.com/#!/rubrics/2262/view)  |<ul><li>[x] </li></ul>|


### Additional
- [ ] Make a better web app
The web app that you make in this project simply reports to the user whether the predicted sentiment was positive or negative. Can you think of a better web app that uses the same model?
- [ ] Improve the web app appearance
The provided web app is very simple and there is plenty of room for improvement if you wish to stretch your web developer skills.
- [ ] Improve the model
The model chosen here is a straightforward rnn with a single hidden layer. There are many different model architectures that you could try to see if they improve the results.

# More details

[Sentiment Analysis Web App](https://github.com/udacity/sagemaker-deployment/tree/master/Project) is a notebook and collection of Python files to be completed. The result is a deployed RNN performing sentiment analysis on movie reviews complete with publicly accessible API and a simple web page which interacts with the deployed endpoint. This project assumes that you have some familiarity with SageMaker. Completing the XGBoost Sentiment Analysis notebook should suffice.

## Setup Instructions

The notebooks provided in this repository are intended to be executed using Amazon's SageMaker platform. The following is a brief set of instructions on setting up a managed notebook instance using SageMaker, from which the notebooks can be completed and run.

### Log in to the AWS console and create a notebook instance

Log in to the AWS console and go to the SageMaker dashboard. Click on 'Create notebook instance'. The notebook name can be anything and using ml.t2.medium is a good idea as it is covered under the free tier. For the role, creating a new role works fine. Using the default options is also okay. Important to note that you need the notebook instance to have access to S3 resources, which it does by default. In particular, any S3 bucket or objectt with sagemaker in the name is available to the notebook.

### Use git to clone the repository into the notebook instance

Once the instance has been started and is accessible, click on 'open' to get the Jupyter notebook main page. We will begin by cloning the SageMaker Deployment github repository into the notebook instance. Note that we want to make sure to clone this into the appropriate directory so that the data will be preserved between sessions.

Click on the 'new' dropdown menu and select 'terminal'. By default, the working directory of the terminal instance is the home directory, however, the Jupyter notebook hub's root directory is under 'SageMaker'. Enter the appropriate directory and clone the repository as follows.

```bash
cd SageMaker
git clone https://github.com/udacity/sagemaker-deployment.git
exit
```

After you have finished, close the terminal window.

### Open and run the notebook of your choice

Now that the repository has been cloned into the notebook instance you may navigate to any of the notebooks that you wish to complete or execute and work with them. Any additional instructions are contained in their respective notebooks.
