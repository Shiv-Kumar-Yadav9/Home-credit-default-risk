# Home-credit-default-risk
This is my first Kaggle submission.
It classifiers the people taking loan as defaulter or not.

# Dataset
The dataset available was a database consisting of data about the customer regarding the age, salary, house, etc.
The dataset was immense and the task was to classify whether the person is a loan defaulter or nto.

# Analysis
The number of samples of class of interest were few when compared to the number of samples of other class.
The dataset was also found very sparse as most of the values of the dataset were missing or NaN.
The correlation among the various fetures pressent in the dataset was also analyzed to identify the important features in determination of the result.

# Preprocessing
The categorical features were then encoded by LabelEncoder if the unique values were just 2, else dummy columns were generated for each of the category of the column.
The train dataset had some feature encodings that were missing in the test dataset thus those columns were dropped off the train dataset to make the dataset contain same number of columns.
The values in the dataset were scaled down between (-1,1) so that al the features have equal importance in determining the result.

# Approach
I gave two simple approaches to solve the problem.
First was to use a Random forest of 100 trees which were then all trained and used in prediction.
Second approach was to use Logistic Regression to classify is a person is a loan defaulter or not.

# Results
I ended up getting a score of 0.69642 for the RandomForest model.
I would have got me a rank of 6234 if I would have participated in the contest.
Other model based on Logistic Regression was also developed and gave a score of 0.68107 .
