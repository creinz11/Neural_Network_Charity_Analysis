# Neural_Network_Charity_Analysis
## Overview 
Using the skills learned in our Neural Network Module, we were tasked with creating a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. To conduct our analysis, we were provided a CSV from Alphabet Soup. The CSV contained more than 34,000 organizations that have received funding from Alphabet Soup over the years, with a variety of different columns and data to base our analysis off of. During this analysis we had to pre process the CSV into a workable format, construct our neural network and compile and train the model based on our dataset.

## Results
### Data Preprocessing

### Target Variable 

* for this model, our target variable was "Is Successful"

## Model Features & features removed from the Data Set

* Identification information such as the Employee Identification Number (EIN) and Charity Name were removed. Identification information should not have a mateerial impact on the successfulness, and willslow down our model unnecessarily so they were removed. The "Application Type" could have been removed in theory, but in a real world application and with additional context, the application type may have a maeterial impact on a charity's successrate. Given our lack of context on Application type, it was left in the analysis.

* The remaining columns were included as features for the purposes of this model.

### Compiling, Training, and Evaluating the Model

* In our intiial itieration of the model, the first hidden layer had 100 and the second had 30. In addition to proceeding with three hidden layers, we also tested several activation functions for each layer (ReLU and Sigmoid function). The output layers activation function was Sigmoid.

* The target performance for the model was 75%. In our initial analysis, we achieved an accuracy score of 55%. In our second iteration, we increased the number of epochs in our model in an attempt to raise accuracy. In our second model run we achieved an accuracy score of 72.5% which was a substantial improvement. In our third attempt we added a third hidden layer with 25 nodes, but registered a similarly low accuracy score to our first model at 53%.

#### Attempt 1
<img width="720" alt="Screen Shot 2021-07-25 at 6 29 38 PM" src="https://user-images.githubusercontent.com/80016496/126916862-4a396394-9b3b-4678-bb07-5480c318f778.png">

#### Attempt 2
<img width="710" alt="Screen Shot 2021-07-25 at 6 30 34 PM" src="https://user-images.githubusercontent.com/80016496/126916901-9e0ef2eb-7ab7-4cf6-874a-dac34d90fdc3.png">

#### Attempt 3
<img width="717" alt="Screen Shot 2021-07-25 at 6 30 58 PM" src="https://user-images.githubusercontent.com/80016496/126916917-d523bb58-c65e-4dbe-b260-222ad279e805.png">

### Summary: 

The highest accuracy score we were able to achieve was 72.5%. The objective of our model was to identify whether or not a project would be successful with Alphabet Soup. Upon reflecting on the model and areas for improvement, I would recommend continued testing with different activation functions. The largest improvement in accuracy came from the use of more epochs. For future analysis I would recommend increasing the number of epochs intially, and then trying different activiation functions. 
