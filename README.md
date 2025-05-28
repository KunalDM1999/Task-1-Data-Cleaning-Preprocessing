# Task-1-Data-Cleaning-Preprocessing

1 Extracted Title from Name, grouped rare ones, and standardized similar titles.
* Used: pandas string operations.

2 Created FamilySize = SibSp + Parch + 1; dropped SibSp and Parch.
 * Used: pandas.

3 Added Ticket_Freq to represent how many times each ticket appears.
* Used: value_counts() in pandas.

4 Dropped irrelevant columns: PassengerId, Name, Ticket, SibSp, Parch.
* Used: pandas.drop().

5 Binary encoded Sex using OrdinalEncoder (0 for female, 1 for male).
*  Used: sklearn.preprocessing.OrdinalEncoder.

6 One-hot encoded Title and Embarked with drop='first' to avoid multicollinearity.
*  Used: sklearn.preprocessing.OneHotEncoder.

7 Winsorized outliers:

* Age = Mild capping using 1st–99th percentiles

* Fare = Stronger capping using 5th–95th percentiles

8 FamilySize → Used IQR method
 * Used: numpy, pandas, and custom logic.

9 Standardized Age (bell-shaped distribution).
* Used: sklearn.preprocessing.StandardScaler.

10 Normalized Fare and FamilySize (skewed).
* Used: sklearn.preprocessing.MinMaxScaler.

11 Verified transformations with visualizations before and after.
* Used: seaborn, matplotlib.pyplot.
