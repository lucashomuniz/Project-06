# ✅ PROJECT 11

The number of patients with liver disease is constantly increasing due to excessive alcohol consumption, inhalation of harmful gases, ingestion of contaminated food and use of drugs and anabolic steroids. In this project, our goal is to develop a Machine Learning model capable of predicting whether or not a patient will develop liver disease, based on various individual characteristics. This model can be a valuable tool for doctors, hospitals or governments when planning their health budgets and implementing effective prevention policies. The desired result is the classification of the patient in one of the classes, yes or no. To achieve this, we will use supervised classification learning techniques, creating different versions of the model with different algorithms. We'll walk you through the entire end-to-end process, including model building, training, evaluation, and selection. Thus, you will deeply understand how this process works, starting from a business problem until the delivery of a trained model that makes accurate predictions. Throughout the project, we will address issues such as which techniques should be applied at each stage, what is the proper order to use these techniques, and which tools should be employed and at what time. Furthermore, we will discuss how to compare the different versions of the models baseed on five types of algoritms.

Keywords: Python Language, Data Analysis, Machine Learning, Classification Model, Supervised Learning, Logistic Regression, Random Forest, KNN, Decision Tree, SVM, Liver Diseases, Health Budget.

# ✅ PROCESS

Based on the business problem definition and dataframe analysis, it is often difficult to determine which algorithm is ideal for developing the machine learning model. Therefore, the plan is to start an experimentation process, testing several algorithms with different combinations of hyperparameters, thus creating different versions of the models, and later comparing which one had the best performance. Likewise, before starting the project, it is difficult to know what the ideal pre-processing techniques are. Therefore, we will also do an experimentation process in this sense. The data scientist's work is based on experimentation in order to choose the best algorithm, technique and strategy. Initially, the Exploratory Analysis is performed right at the beginning, after loading the data. In this phase, tasks such as data cleaning (removal of duplicates and missing values) and possible specific transformations are performed. The main focus is on understanding the dataframe, visualizing the types of numerical and categorical variables, as well as their distributions, and treating outliers based on boxplots, description tables and frequency counts. In Exploratory Analysis, it is important not to have duplicate rows or duplicate columns (variables), as this would introduce duplicate information and could bias the developed model. The goal is to obtain a generalizable model.

![image](https://github.com/lucashomuniz/Project-11/assets/123151332/f32d3cb0-c6b8-4781-be61-6d9d580c6afe)

The next step is Attribute Engineering, in which deeper transformations are performed, if necessary, and variables can be created or modified. One option at this stage is the Feature Selection, to select the best variables for the Machine Learning process. In addition, an important technique at this stage is the creation of the Correlation Table, which allows identifying possible relationship levels (positive or negative) between the variables, especially analyzing evidence of multicollinearity. The next step is preprocessing, where changes are made to variables that are still in text format to convert them to numbers. In addition, the entire Machine Learning model is organized, including the choice of the main algorithm, label encoding, normalization, standardization and data scaling. A widely used technique in this step is to divide the dataframe into training and testing sets. This is important because the Machine Learning model is trained on the training data and then evaluated on the test data. Once the model is trained, it is not appropriate to present the same data used in training, as the model already knows them. To evaluate the performance of the model, it is necessary to use new data, whose results are already known.

![image](https://github.com/lucashomuniz/Project-11/assets/123151332/2e468d48-0c6b-461f-89aa-3a449d451928)


# ✅ CONCLUSION

There are several Machine Learning algorithms that can be applied to different problems. Let's explore some characteristics of the following algorithms: Logistic Regression, Random Forest, KNN, Decision Tree and SVM.

Logistic Regression is a simple and fast algorithm, especially suited for binary classification problems. It provides probabilistic interpretation of predictions and allows evaluating the influence of each variable. However, Logistic Regression may have limited performance in problems with complex decision boundaries and when classes are unbalanced.

Random Forest is a powerful algorithm consisting of a set of decision trees. It is robust against overfitting, handles unbalanced data well, and is able to identify the most important variables. While effective in many cases, training a large number of trees can be computationally expensive and interpreting the results can be more challenging.

KNN (K-Nearest Neighbors) is a non-parametric algorithm that makes no assumptions about the distribution of the data. It is simple to understand and can be effective in problems with complex decision boundaries. However, its performance can be negatively affected by datasets with many features and the prediction time can be longer due to the search for nearest neighbors.

Decision Tree is an algorithm that is easy to interpret and visualize, allowing the identification of the most relevant characteristics. It can handle categorical and numeric variables and is computationally efficient. However, decision trees can be prone to overfitting and creating an optimal tree can be challenging.

SVM (Support Vector Machines) is an effective algorithm in problems with complex decision boundaries and high dimensionality. It can be used in classification and regression problems, being less susceptible to overfitting. However, the proper choice of kernel and hyperparameters can be crucial and the interpretation of the results can be more difficult than with other algorithms.

Each of these algorithms has specific advantages and disadvantages. The choice of the most suitable algorithm will depend on the context of the problem, the characteristics of the data and the objectives of the project. It is important to consider these aspects and perform experiments to evaluate the performance of each algorithm before making a final decision.

![image](https://github.com/lucashomuniz/Project-11/assets/123151332/dbccb0a6-d952-4d11-a721-509eb49889db)

After comparing the five algorithms, it was found that the Random Forest had the best performance, using the AUC Score criterion. However, there are optimization possibilities considering other criteria, such as the inclusion of more relevant variables, exploration of different hyperparameters, increase in training time and modification of data pre-processing. Machine Learning is a continuous cycle, where it is possible to return to the starting point and start a new optimization cycle. With the best trained model, it is possible to perform predictions for several patients simultaneously, loading a .csv spreadsheet containing their data. After standardization, the results can be saved in another spreadsheet and sent to the business area of the company that requested the analysis.

# ✅ DATA SOURCES

Usaremos como fonte de dados o dataset disponível no link: https://archive.ics.uci.edu/dataset/225/ilpd+indian+liver+patient+dataset
