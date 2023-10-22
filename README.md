### Goal
Given historical data by Lending Club on loans given out to borrowers with information on whether or not the borrower defaulted (charge-off), the goal was to build a model that could predict whether or not a borrower will pay back their loan.

### The Data
This project used a subset of the LendingClub DataSet obtained from Kaggle: https://www.kaggle.com/wordsforthewise/lending-club
LendingClub is a US peer-to-peer lending company, headquartered in San Francisco, California.It was the first peer-to-peer lender to register its offerings as securities with the Securities and Exchange Commission (SEC), and to offer loan trading on a secondary market. LendingClub is the world's largest peer-to-peer lending platform.

### Source
The Project is one of the Capstone project given by Jose Portilla in his Machine Learning Course on [https://www.udemy.com/course/python-for-data-science-and-machine-learning-bootcamp/](Udemy).

### How to run the project
To view this file:
1. Download this repository and unzip it
2. Download the Anaconda distribution of python
3. Launch a new Jupyter Notebook from Anaconda
4. Open the Lending Club Project.ipynb from the browser launch by Jupyter Notebook
5. Run all cells
6. Optional: If you don't have the libaries used install it using !pip install <name of the liberay you dont have>

### Process
First an Exploratory Data Analysis(EDA) was done on the dataset which revealed some interesting observation about the dataset among which are: there was an imbalanced class problem in this dataset, most of the people taking loans belong to the B grade, most loans classified as F & G are not being repaid.

Next the missing data in the dataset was handled. For some features whose missing values were more than 5% they were filled using the mean of a column which correlates with that feature. Missing values in certain features who were not relevant and were not significant were dropped. New features were also engineered from certain features like the address feature.

In the machine learning section, the data was divided into training and testing data, the data was normalised, an Artificial Neural Network was used on the training dataser it consisted of 1 input layer, 1 input layer, 1 output layer. 

The model was then used to predict the test data. The accuracy of the model was 89%, precision on those who didn't pay back their loan was (100%).

### Learning
This project made me really understand the difference between recall and precision. While I had 100% precision on charge off borrower, I wanted to increase the recall but that was the problem it's most time a tradeoff when you increase recall you end up decreasing precision. I also learnt that adding more layers to a Neural Network doesn't necessary equate to a better model performance.

### Further Studies
If you are looking to explore this data more. Please do let me know if you were able to increase the recall significantly while not increasing the precision of charged off borrowers.
