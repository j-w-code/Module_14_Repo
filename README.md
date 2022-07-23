# Machine Learning Trading Bot
## Trading bot analysis

>"Enhance!"

In this report we will cover the findings of our machine learning algorithms, the artifical learning models used, and make reccomendations:

* The purpose of our exercise was to test several machine learning models for best performance given the dataset. 
* Our dataset was a local "emerging_markets_ohlcv" CSV file. 
* Initial steps for the data included importing the data into a Pandas dataframe for manipulation, 
  splitting the dataset into "training" and "testing" datasets for use in modeling, 
  and fitting the dataset to our various models for predictions. 
  
  
## Results

* SVC Model Baseline:
  * Below we will include an image with the graph of the modeling for the baseline dataset.
  The graph shows that the actual returns out-performed that of the initial strategy. This model was far more accurate at signalling "buy" events than it was at signalling "sell events. The date-offset for this initial model was set as 3 months. 
  
  ![<alt text>](https://i.postimg.cc/Ls7cSgs5/baseline-predictions.png)
     
* Logistic Regression Model:
  * Below we will add an image of the Logistic Regression Model results graph. The actual results once again outpace that of the strategy. This time by a higher amount than that of the baseline SVC model. This model had a date-offset set as 6 months. 
    
    
   ![<alt text>](https://i.postimg.cc/d0RpgsfZ/lrm-predictions.png)
   


 * Perceptron Model:
  * Below we will add an image of the Perceptron Model results graph. The actual results once again perform better than the stragtegy indicates. This time by a higher amount than that of the baseline SVC model. This model had a date-offset set as 7 months.    
    
    
   ![<alt text>](https://i.postimg.cc/8PR1TSxD/perc-predictions.png)
    
    
    
    
    
## Summary

In this report we took our lending dataset, split the data into training and testing groups for modeling with a Logistic Regression Model in order to detect healthy ("0") and risky ("1") loan values. 
* Of the two models it appears that the resampled dataset model renders slightly better results when attempting to find and classify the risky loans. 
* Performance of the models does depend on what we are trying to solve for. In this case detecting the amount of fewer risky loans when compared to the overall dataset. 

    To that end the resampled model appears to track the risky ("1") data ever so slightly better than the original dataset and we will reccomend using this model. 
    
    
    