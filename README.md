We will be using Google AI first then Vertex AI

Q1) When to use Google AI vs Vertex AI?
Ans: 
1. Google AI : for workshop like this one for kaggle, where production deployment is not needed. Consider building for prototyping or testing a model. 
2. Vertex AI : Much more complex and uses gcloud cli and APIs associated with service accounts as this is used
for production systems. Think IAM, group access restrictions and API service accounts. Docker hosted as most companies will have such a setup. 
Since at a company, we would have real teams to deal with IAM, and service account requests and setup, not advised for prototyping or POC builds. 


Lets first check out how to use Google AI:
I will be making a single agent and then multi agent. 

1. create new env, i use miniconda you can use just python env as well
    - conda create -n <env_name> python=3.12  #You need 3.12 for cli so I prefer 3.12 as per current version 
    - conda activate <env_name>

2. Once in the creted env
    - pip install google-adk

3. For getting the google AI API key, go here - https://aistudio.google.com/app/apikey, use the account where you want to use the Google AI. 

