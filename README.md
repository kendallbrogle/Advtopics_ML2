# advtopics_ML2

Problem 1 - Algorithmic Performance Scaling

Dataset Summary:

Selected a sufficiently large dataset with more than 50K instances from OpenML.
Provided a summary of the dataset, including the number of features, instances, classes, numerical features, and categorical features.
Determined whether the dataset is balanced.
Plotted the distribution of the number of samples per class.
Data Split and Model Evaluation:

Split the dataset into an 80% training set and a 20% test set.
Generated 10 different subsets of the training set by randomly subsampling 10%, 20%, ..., 100% of the training set.
Trained two different classifiers (Decision Tree and Gradient Boosting) on each subset with default hyperparameters.
Measured the wall clock time to train each model.
Evaluated the accuracy of trained models on the test set.
Reported model accuracy and training time for each of the 10 subsets in a table.
Learning Curve Analysis:

Created learning curves for Decision Tree and Gradient Boosting classifiers.
Plotted the accuracy on the test set against the percentage of the training set.
Compared how accuracy changes with increasing training data for both classifiers.
Training Time vs. Data Size:

Created a chart showing the training time of classifiers as a function of training data size.
Analyzed how the training time scales with an increasing amount of training data for each classifier.
Performance Comparison:

Studied the scaling of training time and accuracy of classifiers using the figures generated in parts 3 and 4.
Compared the performance of classifiers in terms of training time and accuracy.
Provided three main observations, including which classifier gives better accuracy and which has a shorter training time.

Problem 2 - Precision, Recall, ROC

Relationship Between ROC and PR Curves:

Discussed the importance of true negatives in both ROC and PR curves.
Argued why each point on the ROC curve corresponds to a unique point on the PR curve.
Binary Classifier Evaluation:

Selected an OpenML dataset with 2 output classes.
Used two binary classifiers (Adaboost and Logistic regression) to create ROC and PR curves.
Presented two figures containing the ROC and PR curves for each classifier.
Highlighted the point where an all-positive classifier lies in the ROC and PR curves.

Problem 3 - Perceptron

Perceptron Implementation:

Implemented the perceptron algorithm without regularization.
Trained the perceptron on a training dataset with 10 points.
Tested its accuracy on 5000 randomly generated points inside the unit square.
Demonstrated the accuracy of the perceptron model on the test points.
Hinge-Loss Comparison:

Modified the loss function from perceptron criterion to hinge-loss.
Repeated the accuracy computation on the same test points.
Examined the effect of changing the loss function on accuracy.
Test Accuracy Analysis:

Compared the test accuracy between the perceptron with the perceptron criterion and the one with hinge-loss.
Provided insights into which case achieved better test accuracy and reasons for the difference.
Classification Stability:

Discussed the scenarios in which the classification of the same 5000 test instances would not change significantly when using a different set of 10 training points.

Problem 4 - Linear Separability

Linear Separability Analysis:

Analyzed a dataset with two features, x1 and x2, consisting of points belonging to two classes.
Discussed whether the dataset is linearly separable and whether a linear classifier can be trained using x1 and x2.
Utilized a plot to argue the linear separability of the dataset.
1-Dimensional Representation:

Defined a new 1-dimensional representation, z, based on x1 and x2, making the dataset linearly separable.
Showed the dataset plot in the z-space to illustrate the linear separability in this 1-dimensional representation.
Separating Hyperplane:

Discussed the appearance and characteristics of the separating hyperplane in the 2-dimensional space.
Nonlinear Transformations:

Explained the importance of nonlinear transformations in classification problems and how they can enable linear separability when the original features are not linearly separable.
