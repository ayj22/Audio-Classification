# Number_Classification


Introduction:

In this assignment we are going to implement Generalized Linear algorithm to identify the character in the given dataset. It is called as flexible generalization of ordinary linear regression is an adaptable speculation of conventional direct logistic regression that considers reaction factors that have mistaken appropriation models other than an ordinary dissemination. The GLM sums up straight logistic regression by permitting the direct model to be identified with the reaction variable by means of a connection work and by permitting the greatness of the change of every estimation to be an element of its anticipated worth. (Wikipedia)

As we have the dataset with instance of digits 0 to 9 already been converted into to pixel. Our aim is to train the model using training dataset and predict the values of testing set. 

The problem statement for the below work is obtained from ( https://drive.google.com/drive/folders/1S5h5Oby5H46u6RZWrCVwuMMIk9pYEdb?usp=sharing ) the dataset used for the problem and python code used for the code has been uploaded in the google folder. In the following step we are importing all the required libraries based on requirement of the assignment

  

We have given data of MNIST in csv format. The dataset consists of around 9999 rows and 784 columns. Values of pixel are in between 0 to 255
 

Here after we have selected the labels of pixel from train set and made the dummy variable in which all the values under the range will be 0 only the true value will have 1 under it.
 
 

In this step we are using the for loop to build 10 model for every digit from 0 to 9. We have used sklearn linear model logistic regression model to train this model. There were several warnings presenting while running just to hide them we have used warning filter function in the beginning. While modelling the model we were getting warnings to increase the maximum iteration which significs number of times we want to iterate values in the model. Secondly, to set the parameter penalty which is used to penalize the model while modeling. [1]
 

In this step we have formatted the probability predictions of the test dataset in the form of data frame after transposing. In the results it is showing as the probability of the respective digit with the highest value under it.


The SoftMax function or standardized outstanding function is a speculation of the strategic capacity to various measurements. It is utilized in multinomial logistic regression and is frequently utilized as the last initiation capacity of a neural networks.

The SoftMax work takes as info a vector z of K genuine numbers and standardizes it into a likelihood conveyance comprising of K probabilities corresponding to the exponentials of the information numbers. That is, before applying SoftMax, some vector parts could be negative, or more noteworthy than one and probably won't entirety to 1 yet in the wake of applying SoftMax, every segment will be in the stretch display in between (0,1), and the segments will amount to. Besides, the bigger info parts will compare to bigger probabilities.[3] 


In the below step we are creating the list of maximum probability by defining max probability function
 

Conclusion:
After performing all the methods and function our model has predicted the accuracy of 91.8% on the testing data. Other than that, we have confusion matrix table which is used to describe the performance of a classification model after applying the built model on the testing dataset.
 
Confusion matrix explains the True Positive, True Negative, False Negative, and True Negative



References:

[1] Sklearn. linear_model.LogisticRegression  https://bit.ly/3oS64tT
[2] Statistical Model Projects https://bit.ly/3cGkfjl
[3] Softmax function https://en.wikipedia.org/wiki/Softmax_function




