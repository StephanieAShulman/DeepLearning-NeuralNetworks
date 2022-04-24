
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

### Summary

