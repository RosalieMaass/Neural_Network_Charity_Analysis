# Neural_Network_Charity_Analysis

## Analysis
- The purpose of this analysis is to help Alphabet Soup predict which organizations are worth donating to and which are too high risk.

## Results
### Data preprocessing:
-   The IS_SUCCESSFUL column is the target for this model
-   All other columns that were not dropped are the features for this model
-   The variable that was neither a target nor a feature is the EIN column and it is removed.
    - Note: In the first few steps it has us remove the "NAME" column, but we later learn that the name column is important and should have been a feature for this model.
### Compiling, Training, and Evaluating the Model
  - I selected 2 hidden layers for my neural network because I didn't want to start too big, and used 42 nodes for the first layer because that's how many columns there is in our data. I used 5 nodes for the second layer. 
  - I was able to acheive the target model performance. 
  - My first model resulted in a 72% accuracy, so I then re-added the "NAME" column and information. I then re-ran the model with the same hidden layers and neurons and got 78% accuracy.

## Summary
- In summary, we know that the "NAME" column provides some valuable information and needs to be included in the model to provide the most relavent information. 
- Another option is to choose different values when binning the information. This may result in changing the number of neurons and hidden layers in the model as well.
