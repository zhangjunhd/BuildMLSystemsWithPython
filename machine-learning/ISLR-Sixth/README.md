# An Introduction to Statistical Learning
![cover](https://img1.doubanio.com/lpic/s28340848.jpg)

    作者: Gareth James / Daniela Witten / Trevor Hastie / Robert Tibshirani 
    出版社: Springer
    副标题: with Applications in R
    出版年: 2013-8-12
    页数: 426
    定价: USD 79.99
    装帧: Hardcover
    ISBN: 9781461471370

[豆瓣链接](https://book.douban.com/subject/21706191/)

- [2.Statistical Learning](StatisticalLearning.ipynb)
    - 2.1 What Is Statistical Learning?
        - 2.1.1 Why Estimate f?
            - Prediction
            - Inference
        - 2.1.2 How Do We Estimate f?
        - 2.1.3 The Trade-Off Between Prediction Accuracy and Model Interpretability
        - 2.1.4 Supervised Versus Unsupervised Learning
        - 2.1.5 Regression Versus Classification Problems
    - 2.2 Assessing Model Accuracy
        - 2.2.1 Measuring the Quality of Fit
        - 2.2.2 The Bias-Variance Trade-Off
        - 2.2.3 The Classification Setting
- [3.Linear Regression](LinearRegression.ipynb)
    - 3.1 Simple Linear Regression
        - 3.1.1 Estimating the Coefficients
        - 3.1.2 Assessing the Accuracy of the Coefficient Estimates
        - 3.1.3 Assessing the Accuracy of the Model
            - Residual Standard Error
            - R2  Statistic
    - 3.2 Multiple Linear Regression
        - 3.2.1 Estimating the Regression Coefficients
        - 3.2.2 Some Important Questions
            - One: Is There a Relationship Between the Response and Predictors?
            - Two: Deciding on Important Variables
            - Three: Model Fit
    - 3.3 Other Considerations in the Regression Model
        - 3.3.1 Qualitative Predictors
            - Predictors with Only Two Levels
            - Qualitative Predictors with More than Two Levels
        - 3.3.2 Extensions of the Linear Model
            - Removing the Additive Assumption
            - Non-linear Relationships
        - 3.3.3 Potential Problems
            1. Non-linearity of the Data
            2. Correlation of Error Terms
            3. Non-constant Variance of Error Terms
            4. Outliers
            5. High Leverage Points
            6. Collinearity
    - 3.6 Lab: Linear Regression
        - 3.6.1 Libraries
        - 3.6.2 Simple Linear Regression
        - 3.6.3 Multiple Linear Regression
        - 3.6.4 Interaction Terms
        - 3.6.5 Non-linear Transformations of the Predictors
        - 3.6.6 Qualitative Predictors
- [4.Classification](classification.ipynb)
    - 4.3 Logistic Regression
        - 4.3.1 The Logistic Model
        - 4.3.2 Estimating the Regression Coefficients
        - 4.3.3 Making Predictions
        - 4.3.4 Multiple Logistic Regression
        - 4.3.5 Logistic Regression for >2 Response Classes
    - 4.4 Linear Discriminant Analysis
        - 4.4.1 Using Bayes’ Theorem for Classification
        - 4.4.2 Linear Discriminant Analysis for p = 1
        - 4.4.3 Linear Discriminant Analysis for p >1
        - 4.4.4 Quadratic Discriminant Analysis
    - 4.6 Lab: Logistic Regression, LDA, QDA, and KNN
        - 4.6.1 The Stock Market Data
        - 4.6.2 Logistic Regression
        - 4.6.3 Linear Discriminant Analysis
        - 4.6.4 Quadratic Discriminant Analysis
        - 4.6.5 K-Nearest Neighbors
        - 4.6.6 An Application to Caravan Insurance Data
- [5.Resampling Methods](resampling.ipynb)
    - 5.1 Cross-Validation
        - 5.1.1 The Validation Set Approach
        - 5.1.2 Leave-One-Out Cross-Validation
        - 5.1.3 k-Fold Cross-Validation
        - 5.1.4 Bias-Variance Trade-Off for k-Fold Cross-Validation
    - 5.2 The Bootstrap
    - 5.3 Lab: Cross-Validation and the Bootstrap
        - 5.3.1 The Validation Set Approach
        - 5.3.2 Leave-One-Out Cross-Validation
        - 5.3.3 k-Fold Cross-Validation
        - 5.3.4 The Bootstrap
- [6.Linear Model Selection and Regularization](LinearModelSelectionAndRegularization.ipynb)
    - 6.1 Subset Selection
        - 6.1.1 Best Subset Selection
        - 6.1.2 Stepwise Selection
        - 6.1.3 Choosing the Optimal Model
            - Cp, AIC, BIC, and Adjusted R2
            - Validation and Cross-Validation
    - 6.2 Shrinkage Methods
        - 6.2.1 Ridge Regression
            - Why Does Ridge Regression Improve Over Least Squares?
        - 6.2.2 The Lasso
    - 6.3 Dimension Reduction Methods
    - 6.4 Considerations in High Dimensions
        - 6.4.1 High-Dimensional Data
        - 6.4.2 What Goes Wrong in High Dimensions?
    - 6.5 Lab 1: Subset Selection Methods
        - 6.5.1 Best Subset Selection
        - 6.5.2 Forward and Backward Stepwise Selection
        - 6.5.3 Choosing Among Models Using the Validation Set Approach and Cross-Validation
    - 6.6 Lab 2: Ridge Regression and the Lasso
        - 6.6.1 Ridge Regression
        - 6.6.2 The Lasso
    - 6.7 Lab 3: PCR and PLS Regression
        - 6.7.1 Principal Components Regression
        - 6.7.2 Partial Least Squares
- [7.Moving Beyond Linearity](MovingBeyondLinearity.ipynb)
    - 7.1 Polynomial Regression
    - 7.2 Step Functions
    - 7.3 Basis Functions
    - 7.4 Regression Splines
        - 7.4.1 Piecewise Polynomials
        - 7.4.2 Constraints and Splines
    - 7.5 Smoothing Splines
    - 7.6 Local Regression
    - 7.7 Generalized Additive Models
        - 7.7.1 GAMs for Regression Problems
        - 7.7.2 GAMs for Classification Problems
    - 7.8 Lab: Non-linear Modeling
        - 7.8.1 Polynomial Regression and Step Functions
        - 7.8.2 Splines
        - 7.8.3 GAMs
- [8.Tree-Based Methods](Tree-BasedMethods.ipynb)
    - 8.1 The Basics of Decision Trees
        - 8.1.1 Regression Trees
        - 8.1.2 Classification Trees
        - 8.1.3 Trees Versus Linear Models
    - 8.2 Bagging, Random Forests, Boosting
        - 8.2.1 Bagging
        - 8.2.2 Random Forests
        - 8.2.3 Boosting
    - 8.3 Lab: Decision Trees
        - 8.3.1 Fitting Classification Trees
        - 8.3.2 Fitting Regression Trees
        - 8.3.3 Bagging and Random Forests
        - 8.3.4 Boosting
- [9.Support Vector Machines](SupportVectorMachines.ipynb)
    - 9.1 Maximal Margin Classifier
        - 9.1.1 What Is a Hyperplane?
        - 9.1.2 Classification Using a Separating Hyperplane
        - 9.1.3 The Maximal Margin Classifier
        - 9.1.4 Construction of the Maximal Margin Classifier
        - 9.1.5 The Non-separable Case
    - 9.2 Support Vector Classifiers
        - 9.2.1 Overview of the Support Vector Classifier
        - 9.2.2 Details of the Support Vector Classifier
    - 9.3 Support Vector Machines
        - 9.3.1 Classification with Non-linear Decision Boundaries
        - 9.3.2 The Support Vector Machine
        - 9.3.3 An Application to the Heart Disease Data
    - 9.4 SVMs with More than Two Classes
        - 9.4.1 One-Versus-One Classification
        - 9.4.2 One-Versus-All Classification
    - 9.5 Relationship to Logistic Regression
    - 9.6 Lab: Support Vector Machines
        - 9.6.1 Support Vector Classifier
        - 9.6.2 Support Vector Machine
        - 9.6.3 ROC Curves
        - 9.6.4 SVM with Multiple Classes
        - 9.6.5 Application to Gene Expression Data
- [10.Unsupervised Learning](UnsupervisedLearning.ipynb)
    - 10.2 Principal Components Analysis
        - 10.2.1 What Are Principal Components?
        - 10.2.2 Another Interpretation of Principal Components
        - 10.2.3 More on PCA
    - 10.3 Clustering Methods
        - 10.3.1 K-Means Clustering
        - 10.3.2 Hierarchical Clustering
    - 10.4 Lab 1: Principal Components Analysis
    - 10.5 Lab 2: Clustering
        - 10.5.1 K-Means Clustering
        - 10.5.2 Hierarchical Clustering
    - 10.6 Lab 3: NCI60 Data Example
        - 10.6.1 PCA on the NCI60 Data
        - 10.6.2 Clustering the Observations of the NCI60 Data