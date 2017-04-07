# Titanic: Machine Learning from Disaster
This is my first Kaggle machine learning "competition". My goal is to play with classic data to improve my analytic skills and learn from what others are doing with the same data. Getting experience in the data world nowadays is simple since public data are widely available. Starting from the data from 1912 means I am a little behind compared to other data scientists. But it is still the first step.

## The Data
|Variable	|Definition|
|---|---|
|survival|	Survival	(0 = No, 1 = Yes)|
|pclass|	Ticket class	(1 = 1st, 2 = 2nd, 3 = 3rd)|
|sex|   Sex	
|Age|	Age in years	|
|sibsp|	# of siblings / spouses aboard the Titanic|	
|parch|	# of parents / children aboard the Titanic|
|ticket|	Ticket number	|
|fare|	Passenger fare	|
|cabin|	Cabin number	|
|embarked|	Port of Embarkation|

### Variable Notes

pclass: A proxy for socio-economic status (SES)
1st = Upper
2nd = Middle
3rd = Lower

age: Age is fractional if less than 1. If the age is estimated, is it in the form of xx.5

sibsp: The dataset defines family relations in this way...
Sibling = brother, sister, stepbrother, stepsister
Spouse = husband, wife (mistresses and fiancés were ignored)

parch: The dataset defines family relations in this way...
Parent = mother, father
Child = daughter, son, stepdaughter, stepson
Some children travelled only with a nanny, therefore parch=0 for them.

In our analysis, the survival outcomes (0 or 1) were the response for our classification study.

# Exploratory Data Analysis
I performed exploratory analysis on the data to investigate different features such as age, gender, class, and fare that could affect the survival outcomes. The jupyter notebook provides our intersting findings. To summarize the results:
* Young children and older adults had a higher rate than that of young adults and elderly.
* Survival rate among female passengers was significantly higher than that of male
* Passengers who paid more in fare were likely to get a better class and had bettter chance of surviving

# Modeling
I constructed two basic models for *logistic regression* and *random forest classification*. The efficacy of the models was assessed by the accuracy, precision and recall scores.
