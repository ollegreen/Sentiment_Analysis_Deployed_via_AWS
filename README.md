# Deploying a Sentiment Analysis Model through AWS Sagemaker

## End result: 
- A web app that you can insert a movie review and the algorithm will tell you if it was positive or negative, based on a Pytorch LSTM classifier model. 
- The model was deployed using AWS SageMaker and could be used in production if it would be inteeresting.
![Sentiment](https://miro.medium.com/max/860/1*Xj8-Jpi5TppZHA8dFRml6A.jpeg)

### Insights from the project: 
- Hyperparameter tuning with AWS: Commonly a pretty time consuiming process, but the gotta say that AWS had some great functionality in SageMaker to help automate this process so we can spend less time on it and in a real life business case could possibly reduce total cost. 


### Libraries used in the project

The list below represents main libraries and its objects for the project.

- Amazon SageMaker (Build, train, and deploy a model)
- PyTorch (LSTM classifier / Recurrent Neural Network)

### The steps taken:
Step 1: Downloading the data
Step 2: Preparing and Processing the data
Step 3: Upload the data to S3
Step 4: Build and Train the PyTorch Model
Step 5: Testing the Model
Step 6: Deploying the model for testing
Step 7: Use the model for testing
Step 6 (again): Deploy the model for the web app
Step 7 (again): Use the model for the web app

## NOTE
- All files are not in the repo, as to deploy the full application there were a lot of Sagermaker specific files. Therefore, just the jupyter notebook showing the end results is showcased in this github repo. 
