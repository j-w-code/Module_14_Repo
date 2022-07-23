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

In this analysis we took our dataset, split the data into training and testing groups, scaled the data, and ran various models to determine which functioned the best.   

* Of all the models used it appears the inital baseline model SVC has results in "Strategy Returns" most closely aligning with "Actual Returns". 
* Both LRM and Perceptron models have higher "Actual Returns" and show high divergence with the projected "Strategy Returns." 
    
    
Given that the alignmnet between "Actual" and "Strategy" returns occurs most closely in the SVC baseline model we will reccomend it's use overall. Although the "Actual Returns" of the other two models is compelling their heavily decoupled "Strategy" status may mean that they are not the best models to be utilized for our purposes. 
    
## Contributors

Jeffrey J. Wiley Jr

## License

MIT
    
    
