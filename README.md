
# Neural Network Charity Analysis
Implementing neural networks using the TensorFlow platform in Python

![NN_skynetToday](https://user-images.githubusercontent.com/30667001/164915952-eb8668b3-b8b1-4c6c-97de-d926eae2e063.png)

### Resources
- Data Sources: Alphabet Soup Charity dataset (charity_data.csv)
- Software: Python 3.7.6, Visual Studio Code 1.65.0, Jupyter Notebook 6.4.5 
- Libraries: TensorFlow, Pandas, Scikit-learn

### Project Overview 

### Results
#### A. Data Preprocessing

|                   | Variable(s)                                                                                     |
|-------------------|-------------------------------------------------------------------------------------------------|
| Target            | Is Successful                                                                                   |
| Features          | Application Type, Affiliation, Classification Use Case, Organization, Income Amount, Ask Amount |
| Neither (Removed) | EIN, Name, Status, Special Consideration                                                        |

* From a total of 12 variables, the target was defined success following funding.
* Four variables were dropped due to lack of benefit (EIN, name) or importance (status, special consideration) in the overall model.
* The remaining features were incorporated into the model.

#### B. Compiling, Training, and Evaluating the Model
![NN_model](https://user-images.githubusercontent.com/30667001/164988809-a77d9642-b896-4f0e-a8cd-5ec1c4676167.png)

![NN_Table](https://user-images.githubusercontent.com/30667001/164989763-d98f7a60-2b71-435b-b308-fd9fd31fa282.png)

- The original model achieved 73% accuracy with a total of 403 parameters run in 100 epochs.
- NN model accuracy was compared to that of Logit, SVM and Random Forest models.
- SVM and RF attained similar accuracy, although all failed to reach the 75% target.
- Although feature reduction is an option for optimizing the NN model, it is difficult to determine using neural networks. Random Forest findings were used, and two additional features were removed from the model.
- Layers and nodes were increased, epochs were increased and decreased and activation was changed, alongside feature reduction.
- It became apparent that an epoch of at least 100 was necessary for model performance, but an increase above that number did not improve performance.
- Despite all attempts, an accuracy above 73% was never realized.

### Summary
Neural network hidden layers are good at uncovering important features, especially when dealing with a great deal of variables. This dataset, however, was more limited. Over 65% of modeling could be captured by three features alone (amount requested, being independently affiliated and company affiliated) as uncovered in the feature importance review. Additionally, the resources to run both the NN and SVM models were more considerable than that of RF, yet all achieved similar accuracy. In this instance, the simpler approach is likely better. Next steps should include finding ways to optimize the RF approach, such as increasing the number of trees.

