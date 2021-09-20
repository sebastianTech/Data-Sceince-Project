# Data-Sceince-Project
Wine Quality (Red) Data Mining Dymistify
he Objectives of CRISP-DM is to understand from a business perspective, what the client really intend to accomplish which is the business goals,availability of resources,the underlying constraints and translate these goals and restrictions into a data mining problem definition. CRISP-DM provides a preliminary plan to achieve the data mining goals and the business goals. The output will have the following:

Phase 1 : Business Understanding.

The business context of our data set is to describe and advise on the best option that

● Gives the vintner the understand behind the science of wine making and align their product to meet consumer’s needs and wants.
● Presents insights into which areas vintner should focus their attention
● Gives the vintner a hint on consumer’s likelihood, preference and willingness to purchase wine with a specific physico-chemical mixture.
● Will give an edge to the producers over other competitors.

Two public datasets that are concerned with the quality of wine are known as “Red and White” from wine samples. Our focus in this project is the Red sample variants from Portugal’s “Vinho Verde” wine and we will be using the python language system for the formulation of this project. The data set has an input (PH value) and output (grading) formulated by experts by assigning the quality values ranging from 3 to 8, where three means terrible, and eight means excellent. There are 1599 observations and 12 attributes. During the per-processing stage, we will discuss the correlation observed with the attributes and apply feature selection. Input variables based on the physico-chemical test in the datasets are

a) Fixed Acidity b) Volatile Acidity c) Citric Acid d) Residual e) Chlorides f) Free Sulphur dioxide g) Total Sulphur dioxide h) Density i) pH j) Sulphates k) Alcohol

Let’s import our wine quality(Red) data set and the needed python libraries:
Image for post
Image for post

Let’s print the first five rows of the data set:
Image for post
Image for post

Understand the variables in your data set and consider thosee that will aid in achieving the business goals while also identifying the data types. In this data set, the quality column will be a key variable or target variable because we would like to know what physico-chemical construct that makes up a good quality wine based on our quality variable’s range of 3 – 8 . All the python codes can be seen with the link https://github.com/sebastianTech/Data-Science-Project.git
Image for post
Image for post

Phase 3 Data Preparation

This is the phase where 80% of the work is done. Some call it data wrangling. In our data set we check for missing values, outliers, standardization (data from difference sources may have different formats), that is applied. Normalization (transforming values in several variables into similar range). The list can continue. It all depends on your business and data understanding that will determine your data pre-processing options. All data pre-processing in this project can be seen via the aforementioned github link.

Binning (process of transforming continuous numerical variables into discrete categorical variables). The quality scale of 3–8 was categorized as Poor, Good and Superior. Quality 3–4(Poor), Quality 5–6(Good), Quality 7–8(Superior).
Image for post
Image for post
Image for post
Image for post

Analyzing individual features and patterns in order to understand the relationships since our target variable is a categorical datatype.
Image for post
Image for post

To visualize the relationships we would use box plot as it is the best way to examine variable correlations. You will observe the variables that makes wine quality, poor or superior. The correlation with its P-value of all the variables were calculated. All can be seen with this link.https://github.com/sebastianTech/Data-Science-Project.git. It was seen that these variables, Sulphate, Citric acid, fixed acidity and Alcohol all have an effect on the correlation and therefore affects the quality of wine.

Phase 4: Data Modelling

Data mining process is a non-linear process hence the understanding you have from your data and business will determine the best modelling techniques to be applied. Here I used Logistic regression, Decision tree, KNN classifier and Linear discriminate analysis. A deep understanding is a prerequisite to this stage. Here we create the Test and Training design
Image for post
Image for post
Image for post
Image for post

Decision Tree accuracy on training set: 1.00
 Decision Tree accuracy on test set: 0.80Logistic regression classifier accuracy on training set: 0.83
Logistic regression classifier accuracy on test set:: 0.84

Phase 5: Model Evaluation

This is where the 4 model used will be assessed in relation to the business objectives. All Model result and assessment will be summarized including a final statement. The model that meets the business success criteria will be selected. Check github account https://github.com/sebastianTech/Data-Science-Project.git, to see the result of the model and why Decision tree was the best Model for this project.

Phase 6: Deployment

Deployment is the last stage of the Cross-Industry Standard. It is crucial and important because no matter how your model looks, the main idea of data mining is to affect decision making positively and increase productivity .

The deployment phase includes four tasks. These are:

Deployment planing (your methods for integrating data-mining discoveries into use)

Planning monitoring and maintenance

Reporting final results(In this case, your recommendations to winemakers based on your findings, the physicochemical variables that needs to improve for a better vinification)

Reviewing final results.

Conclusion

The objective of any vintner is to increase productivity wherever it is necessary and beneficial to their growth. It is our believe that with the information provided throughout this project, it can aid in the decision making or vintners especially when it concerns the physio construct of a wine, and the where they main focus should be in terms of wine quality. We can see from preliminary observations, that the wine quality labeled as “Good” had the highest and most predominant occurrence which seems to suggest that most customers buy wine of that range giving vintners an idea of the type of wine they should focus on. In time these observations can change as people and societies evolve but to understand it’s effect is what this project is seeking to satisfy.
