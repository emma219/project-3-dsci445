# project-3
Class project for group 3 in DSCI445 @ CSU

Team Members: Megan Dunnahoo, Mandey Brown, Emma Hamilton

Group3_Project.Rmd is our RMarkdown file with all of our code

Slides.Rmd is our RMarkdown file for our presentation

In Group3_Project.Rmd the first chunk contains all libraries needed for the code to execute. set.seed(445) was then used for reproducibility

Motivation and Methodology for the project, to predict the Sale Price of Homes in Ames Iowa using the data provided from Kaggle were explained. 

Once the training and test data from Kaggle was uploaded, NA values in the  data were addressed in the training data. All categorical values that contained NA (with the exception of one variable) in the training data were variables where an NA could occur based on the lack of the presence of the aspect were possible, as such another level was created for None. All missing values in the continuous data was replaced with 0. 

Once missing values were handled a visual exploration of that training data was completed using a variety of ggplot functions and approaches.

During the visual exploration it appeared that the Sale Price (the variable of interest) was right tailed skewed. The variable was then log transformed to account for that. 

The training data was then split into training and test data for model exploration. A 70/30 split was used. 

The following models were then fit and a MSE was calculated for each:
Decision Tree
Random Forest
Bagged Tree
Boosted Tree
LASSO

A table was produced that contained the model and MSE value.

One the ideal model was determined. Given the complexity, interpretability, and MSE values, the Random Forest model appeared to be the best option.

The test data provided from Kaggle was then addressed. It was prepossessed so that it would be similar to the training data also provided from Kaggle. 

