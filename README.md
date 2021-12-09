
# Mental-Or-Physical-Disease-Treatment

As we know that good mental and physical health plays very important role in our life 
because the society always judge us by our behaviour and behaviour comes
from our mental health. For doing good amount of production activity or work
we need mental and physical health. If we have one then can perform any
task.

In this project we have to fimd whether all employees have good health 
So in this we have to find which employee need mental treatment or physical 
treatment or both.
## Data Analysis

In Mental-Or-Physical-Disease-Treatment dataset we are provided 27 features(including target 
variable) and 1258 records.

* Timestamp: Date of checkup
* Age: Age of employees
* Gender: Gender of Employees
* Country: Employees belong to respective Country
* state: Employees belong to respective state
* self_employed: working for oneself as a freelance or the owner of a business rather than for an employer.
* family_history: IS the same treatment given to family or not
* work_interfere: how do they work
* no_employees: number of employees
* remote_work: whether employees work from office or they work form home 
* tech_company: what kind of organization techinical or non technical
* benefits: benefits of employees
* care_options: care of optics
* wellness_program: wellness of employees
* seek_help: seek help taken by employees
* anonymity: anonymity in employees
* leave: employess on leave or not
* mental_health_consequence: mental health of employees
* phys_health_consequence: physical health of employees
* coworkers: employees are coworker or not 
* supervisor: empployess are supervisor or not
* mental_health_interview: mental health inteview is done or not
* phys_health_interview: physical health interview is done or not
* mental_vs_physical: Al their health of employees is good or not
* obs_consequence: observation on employees
* comments: comments on observation
* treatment: Is any treatment need for employees
## Approach

Our Main goal is to know that whether which applicant 
it belong to defaulter or non-defaulter.

* Data Exploration : Exploring dataset using pandas,numpy,matplotlib and seaborn.
* Data visualization : Use Tableau Data visualizationtools and also Ploted graphs to get insights about dependend and independed variables.
* Model Selection I : Tested all base models to check the base accuracy. Also ploted and calculate Performance Metrics to check whether a model is a good fit or not.
* Model Selection II : After testing all base if some of them are not working properly then we have to do model tunning
* Pickle File : Selected model as per best accuracy and created pickle file using pickle library.
* Webpage & deployment : Created a webform that takes all the necessary inputs from user and shows output. After that I have deployed project on Herokuapp 

## Technologies Used

* Jupyter notebook, Spyder, VScode Is Used For IDE.
* For Visualization Of The Plots Matplotlib , Seaborn Are Used.
* Git Hub Is Used As A Version Control System.
* os is used for creating and deleting folders.
* csv is used for creating .csv format file.
* numpy is for arrays computations and mathematical operations
* pandas is for Manipulation and wrangling structured data
* scikit-learn is used for machine learning tool kit
* pickle is used for saving model
* Logistic Regression is used for LogisticRegression Implementation.
* SGDClassifier is used for SGDClassifier Implementation.
* KNeighborsClassifier Regression is used for K-Nearest Neighbors Implementation
* SVC is used for Support Vector Machine
* Decision Tree is used for DecisionTreeClassifier Implementation.
* Random Forest is used for RandomForestClassifier Implementation.
* VotingClassifier for Ensemble Modelling

## Conclusion
We have developed Mental-Or-Physical-Disease-Treatment Prediction. This model 
is used to predict whether the employees are undergoing throgh mental or physical health.
For building this model we import training.csv in jupyter notebook using pd.read_csv and we 
check the datatype of every column using info(). After that we have check the missing values
deleted volumns having more than 50% of missing values in respective columns
. And after looking at gender columns values we notice that their are more than
2 gender so we replace all values by Males, Females and nan values after we have treated
missing values by mode because gender is categorical column. And done same for 
other numerical column from mean, and categorical column from mode.
After traeting missing value we have done label encoding.
After that we done Data Visualization first we plot box plot for numerical column
to see whether the outlier is present or not. Here Outliers were absent.
Next step is to build machine learning model befor that we scaled data using StandardScalar
and We build Logisic Regression, SGDClassifier, KNeighborsClassifier, SVM, DecisionTreeClassifier,
RandomForestClassifier, and VotingClassifier out of all decision tree model is best 
among all.
After doing all this step we have to perform all steps for test file but her 
while scaling we don't have to create new object we have to us transform function and not train function
and while predicting we dont have to create same decision tree model we have to 
use predict function not fit function and we can save that model using pickle library
in .sav or .pkl file