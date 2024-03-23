# Project Title

ML Classification for Performance evolution for Engineering Students

## Description

Running various ML classification algorithms on "Data of Academic Performance evolution for Engineering Students";

## Best Results
Winner algorithm: Random Forest;
Accuracy and precision matrix of for 13 classification labels: 75.3%

Accuracy (train) for RFST: 75.3% 
              precision    recall  f1-score   support

           A       0.69      0.78      0.73       894
          A+       0.91      0.85      0.88       910
          A-       0.72      0.63      0.67       937
           B       0.72      0.69      0.70       908
          B+       0.72      0.74      0.73       875
          B-       0.74      0.78      0.76       920
           C       0.72      0.71      0.72       928
          C+       0.75      0.76      0.76       903
          C-       0.75      0.81      0.78       940
           D       0.75      0.74      0.74       922
          D+       0.75      0.81      0.78       926
          D-       0.76      0.81      0.78       907
           F       0.85      0.67      0.75       902


## Outline Process

1. Load the original dataset data_academic_performance.csv
2. Initial exploration to understand data structure, content, missing values, dat types, etc.
3. Data visualisation to understand distribution
4. Create a new column 'GRADE' by converting the 'PERCENTILE' column into labels from A+ to F using Queen's algorithm; it creates 13 lables total
5. Calculate corelations in betwwen features and 'GRADE'
6. Based on corelation score, select the columns left for classification
7. Remove the features to avoid overfitting the model
8. Sort out the 'UNIVERSITY' featrure column by setting a treshold (100) or keeping thr university name or labelling as "Other"
9. Remove zero values from the interest columns
10. Encode the 'QR_PRO', 'CR_PRO', 'CC_PRO', 'ENG_PRO', and 'WC_PRO' (previous marks) columns into categories: A, B, C, D, F
11. Save the dataset into a new .csv file called cleaned_data.csv in same ../Data directory
12. Perform datya analysis on the cleaned dataset
13. Analyse the distribution of labled 'GRADE'
14. Determine the top 10 most influencial factors of the categorical features to 'GRADE'
15. Drop the most common factors that create confusion between distinct grades
16. Convert data, apply SMOTE algorithm, export the data into data_academic_ready.csv file
17. Perform Logistic Regression on ready file
18. Perform other classifiers on the ready file
19. Determine the best accuracy for the models
20. Fine tune best algorithms





### Dependencies

* Python 3.12.1 environment
* Visual Stodio Code, Git, Github
* List Python Libraries used:
    * pandas
    * matplotlib.pyplot
    * seaborn
    * scipy.stats


### Data Collection: 

* Data Source: https://data.mendeley.com/datasets/83tcx8psxv/1
* Excel file converted locally into .csv

### Files in use by the algorithm

All files are placed in ../Data folder of the project workspace structure

* Original file downloaded from source: data_academic_performance.xlxs (Excel format)
* File converted into .csv format to be loaded and utilized by pandas library (simple conmversion using Excel "Save as" function): data_academic_performance.csv
* File cleaned of null values, values not considered, etc.: cleaned_data.cvs
* Final File to be used by classifiers; most common columns used, data transformed: data_academic_ready.csv


### Data Cleaning and Preprocessing:

* Handle missing values: Decide how to handle missing data, either by imputation or removal.
* Encode categorical variables: Convert categorical variables into numerical format using techniques like one-hot encoding.
* Feature scaling: Scale numerical features if necessary to ensure they are on the same scale.
* Remove irrelevant features: Remove features that are not relevant or do not contribute to the classification task.


### Feature Engineering:

* Create new features: Derive new features from existing ones that may be more informative for the classification task.
* Feature selection: Select a subset of features that are most relevant for predicting student grades

### Data Splitting:

* Split the dataset into training and testing sets. The training set is used to train the classification model, while the testing set is used to evaluate its performance.


### Model Selection:

* Choose a suitable classification algorithm for predicting student grades. Common algorithms include logistic regression, decision trees, random forests, support vector machines (SVM), etc.
* Tune hyperparameters: Optimize the parameters of the selected model using techniques like grid search or random search

### Model Training:

* Train the selected classification model on the training data.

### Model Evaluation:

* Evaluate the performance of the trained model on the testing data using appropriate metrics such as accuracy, precision, recall, F1-score, etc.
* Analyze the results and fine-tune the model if necessary.

### Model Training:

* Train the selected classification model on the training data.

### Deployment:

* Once satisfied with the model's performance, deploy it to make predictions on new, unseen data.

Throughout this process, it's important to iterate and refine each step based on the results obtained. Additionally, consider conducting exploratory data analysis (EDA) to gain insights into the data and better understand the relationships between different features and student grades.

```
code blocks for commands
```

## Help

Any advise for common problems or issues.
```
command to run if program contains helper info
```

## Authors

Contributors names and contact info

ex. Dominique Pizzie  
ex. [@DomPizzie](https://twitter.com/dompizzie)

## Version History

* 0.2
    * Various bug fixes and optimizations
    * See [commit change]() or See [release history]()
* 0.1
    * Initial Release

## License

This project is licensed under the [NAME HERE] License - see the LICENSE.md file for details

## Acknowledgments

Inspiration, code snippets, etc.
* [awesome-readme](https://github.com/matiassingers/awesome-readme)

