# Deploying a Sentiment Analysis Model through AWS Sagemaker

## Result: 
- A web app that you can insert a movie review and the algorithm will tell you if it was positive or negative, based on a Pytorch LSTM classifier model. 
- **Picture of the final result can be found in the repo as "final_result.png"**
- The model was deployed using AWS SageMaker and could be used in production if it would be inteeresting.
![Sentiment](https://miro.medium.com/max/860/1*Xj8-Jpi5TppZHA8dFRml6A.jpeg)

### Insights from the project: 
- Hyperparameter tuning with AWS: Commonly a pretty time consuiming process, but the gotta say that AWS had some great functionality in SageMaker to help automate this process so we can spend less time on it and in a real life business case could possibly reduce total cost. 


### Libraries used in the project
The list below represents main libraries and its objects for the project.

- Amazon SageMaker (Build, train, and deploy a model)
- PyTorch (LSTM classifier / Recurrent Neural Network)

#### Why did we use Amazon Lambda? 
We used Amazon Lambda service to “Function as a service (FaaS instead of SaaS)”, instead of creating a server, using this FaaS we were able to tell amazon we need a specific function to run when a specific event occurs. Saves a lot of money as you don’t have to have a server running the whole time, only pay when your function is running. 

#### Why did we use Amazon API Gateway?
We used Amazon API Gateway to manage APIs to back-end systems running on Amazon Lambda. 


### Project steps taken:
1. Downloading the data
2. Preparing and Processing the data
3. Upload the data to S3
4. Build and Train the PyTorch Model
5. Testing the Model
6. Deploying the model for testing
7. Use the model for testing
6. (again): Deploy the model for the web app
7. (again): Use the model for the web app

## NOTE
- All files are not in the repo, as to deploy the full application there were a lot of Sagermaker specific files. Therefore, just the jupyter notebook showing the end results is showcased in this github repo. 
