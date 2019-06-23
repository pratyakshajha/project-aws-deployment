## Project Overview

This repository hosts code used in fifth project on deploying Neural Networks project in the Deep Learning Nanodegree. 

The project involved deploying a RNN based sentiment analysis on movie reviews complete with publicly accessible API and a simple web page which interacts with the deployed endpoint. This project assumes that you have some familiarity with SageMaker.

## Getting started
Open the `Sagemaker Project.ipynb` in a Sagemaker notebook instance(`ml.t2.medium`, a cpu instance is covered in the free tier). Clone this repo into the notebook instance. The notebook consists of further technical details to guide you through the deployment. Run the notebook to your own sentiment analysis webapp.

### Further improvements
- [ ] Make a better web app
The web app that you make in this project simply reports to the user whether the predicted sentiment was positive or negative. Can you think of a better web app that uses the same model?
- [ ] Improve the web app appearance
The provided web app is very simple and there is plenty of room for improvement if you wish to stretch your web developer skills.
- [ ] Improve the model
The model chosen here is a straightforward rnn with a single hidden layer. There are many different model architectures that you could try to see if they improve the results.
