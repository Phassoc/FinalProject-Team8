# Demystifying Machine Learning (ML)
### Final Project
Project Team 8: 
* Lori Shannon
* Philip Hill
* Rob Gauer
# 
# Red Wine Quality 

![MLandWine.PNG](images-README/MLandWine.PNG)
## Objective - Create an analysis of existing data to make a prediction, classification, or regression.
#
## Story - How do the physicochemical factors affect Red Wine quality?
Wine is a (delicious) alcoholic drink that dates back to 5000 BC.

The red-wine production process involves the extraction of color and flavor components from the grape skin. Red wine is made from dark-colored grape varieties.

Winemakers are investing in new technologies to improve the quality of wines. By assessing the most influential factors through physicochemical tests, we can use the outcomes to determine the relationship of the factors to the quality rating of the final wine produced.

After assembling the dataset, we used Python Pandas and Matplotlib to examine existing data on wine quality and then employed machine learning for regressions and predictions. Additionally, we include Tableau vizualizations based on the existing data to show the factors our machine learning models were based on.
 
#
## Analysis
Our team prepared a 15-minute data walktrough of how Machine Learning can describe three different physicochemical factors that affect the quality of red wine. The three physicochemical factors used in the analysis are volatile acidity, pH, and alcohol.

The following Machine Learning methods were used to predict and classify the physicochemical factors:
   
   * Multiple Linear Regression.
      * Simply means that you have more than one feature (independant) variable.
        * The definition of Linear Regression:  A regression line is simply calculating a line that best fits the data. This is typically done through the least squares method where the line is chosen to have the smallest overall distance to the points. (y=mx+b)
      * Residuals (The plots for MLR are called a Residual Plot)
        * Because we can't easily plot our line in 3D space, we can use a residual plot to check our predictions. Residuals are the difference between the true values of y and the predicted values of y. 
          Source: Interpreting Residual Plots. https://www.qualtrics.com/support/stats-iq/analyses/regression-guides/interpreting-residual-plots-improve-regression/    
      * Conclusion: A good R2 Score will be close to 1. The above results individually the model does not predict a solid or good relationship between this factor and quality.
          Overall the individual factors (features) do not individually prove to affect the quality based on their scores. When we view the 'Combined' features they have a more high training and test score. This concludes that the quality is more a factor of the overall physicochemical mixture (formula) of factors than any one individual factors (features).       
      
          	Alcohol - 
            Training Score: 0.23696651674458968
            Testing Score: 0.1910028687215255
            Linear Regression: r-squared is: 0.22673436811123157
              
            pH - 
            Training Score: 0.0011473146969438464
            Testing Score: 0.00600616046948832
            Linear Regression: r-squared is: 0.22673436811123157
              
            Volatile Acidity -
            Training Score: 0.14102234538667047
            Testing Score: 0.18732594098971278
            Linear Regression: r-squared is: 0.22673436811123157
              
            Combined -
            Training Score: 0.31952395893964436
            Testing Score: 0.32870190860224924

   * Logistic Regression.
      * Logistic Regression is a statistical method for predicting binary outcomes from data.
        * Examples of this are "yes" vs "no" or "young" vs "old".
          These are categories that translate to probability of being a 0 or a 1.
      * Conclusion: The classification algorithm used to predict a that the factors (features) used have the greatest signifigance to the set of 'quality' classes equal to 6.
      
           	Alcohol has a higher function on the category of quality = 6.
            Training Data Score: 0.6005004170141784
            Testing Data Score: 0.605
              
            pH has a higher function on the category of quality = 6.
            Training Data Score: 0.6005004170141784
            Testing Data Score: 0.605
              
            Volatile Acidity has a higher function on the category of quality = 6.
            Training Data Score: 0.6005004170141784
            Testing Data Score: 0.605

   * Neural Network.
      * A neural network is a series of algorithms that endeavors to recognize underlying relationships in a set of data through a process that mimics the way the human brain operates. Neural networks can adapt to changing input; so the network generates the best possible result without needing to redesign the output criteria.  
      
      * Our neural network objective was to apply a normal neural network layer of 2 inputs, 6 hidden nodes and 2 outputs to our training data set and then determine whether applying additional deep learning layers (6 additional hidden nodes) to our data set would yield additional predictive insights (training accuracy and loss) relative to red wine quality and the 11 active ingredients (physicochemicals) that contribute to wine quality.

      * Conclusion: We DID benefit modestly from applying a Deep Learning Neural Network to our training data set. As evidenced by the outcomes below, the deep learning model found patterns of less loss and more accuracy with the same levels of active ingredient input as was found in the normal neural network when trying to predict Red Wine quality.


   * Tableau.
      * Tableau can help anyone see and understand their data. It comes with tools that allow to drill down data and see the impact in a visual format that can be easily understood by any individual.
        
        We include Tableau visualizations based on the existing data to show the factors our machine learning models are based on.
#  
## Team Repository
  * https://github.com/hockeylori/FinalProject-Team8
  * Launch the following web link for the project presentation:  
      * https://hockeylori.github.io/FinalProject-Team8/index.html
#
## Data Sources & Information Reference
   * UCI Machine Learning Repository. https://archive.ics.uci.edu/ml/datasets/Wine+Quality 
   * Data source of origin: https://archive.ics.uci.edu/ml/machine-learning-databases/wine-quality/
   * Link: https://archive.ics.uci.edu/ml/machine-learning-databases/wine-quality/winequality-red.csv
   * Attribute Information:
      * Input variables (based on physicochemical tests):
          1 - fixed acidity
          2 - volatile acidity
          3 - citric acid
          4 - residual sugar
          5 - chlorides
          6 - free sulfur dioxide
          7 - total sulfur dioxide
          8 - density
          9 - pH
          10 - sulphates
          11 - alcohol
      * Output variable (based on sensory data):
          12 - quality (score between 0 and 10)
#           
## Requirements Overview
  1. Data & Visualization components used in our project include:
      * Python Flask, HTML/CSS, Python Pandas, Jupyter Notebook, Python Matplotlib, Tableau, and GitHub IO. 
  2. Scikit-Learn and/or another machine learning library.

#
## Functional Work Flow 
  1. Dataset CSV file is reviewed and prepared: ../assets/winequality-red.csv 
  2. Python Jupyter Notebook and Matplotlib plot files for each machine learning technology used.
  3. Tableau used for visualization. Functional review of dataset for quick review of described visualizations.
  4. Published via GitHub IO for presentation of our data visualization of ML components to tell the story.
      * Link:  https://hockeylori.github.io/FinalProject-Team8/index.html
  #
## Visualizations
  * Web site Home Page URL and Selection Dropdown Menus.
    * https://hockeylori.github.io/FinalProject-Team8/index.html
  * Individual visualization files:
    * https://github.com/hockeylori/FinalProject-Team8/tree/master/assets/images

# 
### Data Analytics & Visualization 
 Lori Shannon, Philip Hill, Rob Gauer.
 
### Copyright August 2020
#
![wine-quality.jfif](images-README/wine-quality.jfif)
#
#
# FINAL PROJECT INSTRUCTIONS

![project-three-image.png](images-README/project-three-image.png)

# Demystifying Machine Learning (ML)

## REQUIREMENTS
1. Find a problem worth solving, analyzing, or visualizing.
2. Use ML in the context of technologies learned.
3. You must use: Scikit-Learn and/or another machine learning library.
4. You must use at least two of the below:
    * Python, Pandas, Python Matplotlib, 
    * HTML/CSS/Bootstrap, JavaScript Plotly, JavaScript D3.js, JavaScript Leaflet, 
    * SQL Database, MongoDB Database, 
    * Goodle Cloud SQL, Amazon AWS, Tableau.
5. Host application using Heroku or a tool of your choice.
6. Prepare a 15-minute presentation data deep-dive or infrastructure walkthrough that shows machine learning in the context of what we’ve already learned. 
#
![red-wine-glasses.jfif](images-README/red-wine-glasses.jfif)
# 
### Copyright
Trilogy Education Services © 2019. All Rights Reserved.
# 