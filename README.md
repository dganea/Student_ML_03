# Project Title

ML Classification for Performance evolution for Engineering Students

## Description

Running various ML classification algorithms on "Data of Academic Performance evolution for Engineering Students";

## Outline Process

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

