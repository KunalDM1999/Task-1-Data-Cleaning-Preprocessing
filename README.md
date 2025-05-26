# Task-1-Data-Cleaning-Preprocessing

1 Extracted Title from Name, grouped rare ones, and standardized similar titles.

2 Created FamilySize = SibSp + Parch + 1; dropped SibSp and Parch.

3 Added Ticket_Freq to represent how many times each ticket appears.

4 Dropped irrelevant columns: PassengerId, Name, Ticket, SibSp, Parch.

5 Binary encoded Sex using OrdinalEncoder (0 for female, 1 for male).

6 One-hot encoded Title and Embarked using OneHotEncoder(drop='first').

7 Winsorized outliers:

a Mild capping for Age (1st–99th percentiles),

b Stronger capping for Fare (5th–95th percentiles),

c Used IQR method for FamilySize.

8 Standardized Age (bell-shaped distribution) using StandardScaler.

9 Normalized Fare and FamilySize (skewed) using MinMaxScaler.

10 Verified transformations with distribution plots before and after processing.

