# Neural_Network_Charity_Analysis

### Overview of the Analysis
The purpose of this analysis is to utilize machine learning techniques along with neural networks to assist Alphabet Soup which is a non-profit fund-raising company. Our goal is to create a binary classifier that can predict which candidates will be successful if funded. First we were to preprocess the data for the neural network model. Secondnly we were to compile, train, and evaluate the model. Then we tried to optimize the neural network model. The dataset we are using is called charity_data.csv.

### Results
#### Data Preprocessing

* What variable(s) are considered the target(s) for your model?
I would consider IS_SUCCESSFUL to be the target variable for our model.

* What variable(s) are considered to be the features for your model?
Variables such as APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT, and ASK_AMT are the variables 
I would consider as features for the model.

* What variable(s) are neither targets nor features, and should be removed from the input data?
The variables that are neither targets or features are EIN and NAMe, that is why we removed them from the dataframe.

#### Compiling, Training, and Evaluating the Model

* How many neurons, layers, and activation functions did you select for your neural network model, and why?
My final model had 3 layers, with 80 neurons in the ifrst, 40 in the next and 10 in the final. This is what I went with because after numerous tests these produced my best results for accuracy and loss.

* Were you able to achieve the target model performance?
I was not able to achieve the goal of 75%. Possibly with more optimizing it is possible, but I tried for quite some time, and usually the results were getting worse and not better.

* What steps did you take to try and increase model performance?
The first step I tried was to remove more columns from the dataset, this actually caused the accuracy and loss to go in the wrong direction.
The next step I did was to add more layers. I found this helped some of the time, but also when adding to many layers caused for worse results. I settled on 3 layers. My next effort was adjusting the activation function, I found combinations of Leaky_Relu and Relu were what lead to better numbers. My final optimization was playing around with the numbers of neurons. I found that the higher I went also led to a lower accuracy, but to low was also not good. I found a combination that gave me a higher accuracy than the original test so I took that as a victory.

### Summary 
The initial model had an loss of 0.5634852051734924, and an Accuracy of 0.7282798886299133.
After optimizing the model, we were able to get the results of; Loss: 0.5549336671829224, Accuracy: 0.7294460535049438
We tried countless efforts to get the accuracy to a more acceptable number but could only increase the efficiency slightly. 
The goal was 75% accuracy, and we fell short of that. More computations would have to be made to achieve that goal.

Final Model Results are below.

<img width="399" alt="final_model_results" src="https://user-images.githubusercontent.com/118485409/233744875-a3fa1a18-a7d2-4846-8115-359b207d3651.png">
