# Machine Learning Code Challenge 

Given 2 data challenges that test for the ability to:
- Wrangle/clean data to make it usable by a model
- Figure out how to set up X's and y's for a use case, given a dataset
- Write code to robustly and reproducibly preprocess data
- Pick/design the right model, and tune hyperparameters to get the best performance

#### Deliverables:
- A link to a github repository that contains:
    - Code is documented within the notebooks
    - Models stored with joblib
    - ReadME file:
        - Instructions to easily access/load the above
        - A writeup explaining any significant design decisions and your reasons for making them. 
        - If needed, a brief writeup explaining anything you are particularly proud of in your implementation that you might want us to focus on
    
    
        I've built rough working copies of each task in a separate notebook. There are 3 working copies, task 1, task 2, and the Neural Net.
        The main notebook is the MachineLearningChallenge notebook. It contains a comprehensive functionalized implementation of the code for both the tasks. Including a final "train(data)" and "predict(data)" function. Hyperparameter tuning resulted in models too big for github so I've scaled them back down for space limitations.
        
        For the Neural Network implementation, I explored an LSTM inspired by a similar project. However, with the increase in results, it came with a multitude of complexities. For now, a simple version of models using XGBoost for predictive failure and RandomForestRegression for forecasting have been used. 
        
        If I had to pick, I'd say I'm proud of not having used any for loops at all. Vectorized and package based implementations help with speed and scale! 
        
        Oh, also proud of how much fun I had working through this problem! 
        

#### Code Assessment:
- Accuracy/RMSE of your model when predicting on held-out data
- How well various edge cases are handled when testing on held-out data. For example, if the held-out data contains:
    - A new column that wasn't present in the dataset given to you 
    - New value in a categorical field that wasn't seen in the dataset given to you
    - NA values
    
    Preprocess Functions aims to cover these edge cases
    
- Efficiency of the code. 
    - Is it easy to understand? I think so
    - Are the variable names descriptive? Yes
    - Are there any variables created that aren't used? No 
    - Is redundant code replaced with function calls? Yes
    - Is vectorized implementation used instead of nested for loops? Yes, pandas!  
    - Are classes defined and objects created where applicable? Wasn't applicable, I believe
    - Are packages used to perform tasks instead of implementing them from scratch? Yes, numpy, pandas, scikit-learn, keras
    
  
#### References:
WaterPump Maintenance: https://towardsdatascience.com/water-pumps-maintenance-prediction-data-science-illustrated-20c7100017c5
Hyperparameter tuning: https://towardsdatascience.com/hyperparameter-tuning-the-random-forest-in-python-using-scikit-learn-28d2aa77dd74 
