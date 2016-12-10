# Data-Analysis
Homework Code For My Data Analysis Course, instructed by Jon Walker

## Homework 1 (Law of large number)

Modify the Law of Large Numbers rmd file to

1.  Use a uniform distribution instead of a normal distribution.  The function for a uniform is runif instead of the rnorm.

2.  Change the size of the sample from 10,100, and 1000 to 20, 300, and 4000.

3.  Change the output so that it prints the actual sample mean instead of the difference between the sample mean and the population's mean.

4.  For the biased section, change the rule to if the observation is between .6 and .7 then it is set to a missing value (NA).


## Homework 2

1.  Download the iris data set from courseweb

2.  Delete the setosa iris cases

3.  Keep petal width and sepal width and iris type

4.  Make a dummy variable for iris type

5.  Create a random number, sort the data by that random number

6.  Divide the data (100 obs) into 10 groups based on their order

7.  Take 9 of the ten groups and run a linear regression with petal width as a function of iris type and sepal width

8.  Do that 10 times so that each group of ten obs is omitted from one of the regressions

9.  Keep track of the intercept, dummy variable coefficient, and sepal width coefficient

10. Make a histogram (hist) of those three values (there will be 3 histograms with ten observations in each histogram).


## Homework 3

Using iris dataset

1.  Only using sepal length as a variable, create a 10 fold knn execution with k=5.

2.  From the testing set keep track of what each observation was predicted to be.

3.  Create a confusion matrix of the final results:  what each of the 150 observations was predicted to be vs what it actually is.

4.  Create a density plot of correct and incorrect predictions as a function of sepal length.

## Homework 4

In homework 3, we did a 10 fold cross validation of the iris dataset.  What we are going to do in homework 4, is

1. Read in the iris data set. 

2. Randomly pick 50 observations to be the testing dataset. 

3. Do this loop 100 times: For the remaining 100, take a sample of 100 observations (with replacement) from that 100 and build a model predicting what type of iris the observation is given its sepal width.  

4. Using the model just developed, predict what is the iris type of the each of the 50 held out as the testing dataset.  

5. For each observation in the testing dataset set keep track of how often, it is predicted to be each of the three iris types. 

6. After you have 100 predictions for each of the 50 observations in the testing dataset, decide what iris type each observation is in the testing dataset by voting, each observation is predicted to be whichever type gets the most votes.  If there is a tie randomly choose one or the other. 

7. Create a confusion matrix for these 50 observations.

8. Compare the accuracy rate from this process with what you observed for homework 3.

## Homework 5

Using iris data:

1. Create 'Cost Function': 
   Benefits: Setosa correct 1 point, Veriscolor correct 3 points, Virginica correct 1 point
   Costs: Veriscolor wrong 10 points

2. Determine Best: 1, 2 and 3 variable models using Naive Bayes and some other method.

## Homework 6

1. Create the Reuters dataset.

2. Create a smaller dataset with inspect(removeSparseTerms("your dataset name",0.6)). Be sure to do all the preprocessing: stemming, stop words, etc.

3. Do a hierarchical analysis with however many documents you end up with and plot the tree out.  

4. Go ahead and use a Euclidean distance metric instead of cosine similarity if you want.  
