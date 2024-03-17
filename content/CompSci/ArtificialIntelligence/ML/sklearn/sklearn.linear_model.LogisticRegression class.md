---
mindmap-plugin: basic
tags:
  - CompSci/programming/Python/class
  - CompSci/AI/ML/model/linear/logistic
---
# sklearn.linear_model.LogisticRegression class
### Description:
- Logistic Regression (aka logit, MaxEnt) classifier.
-  [[Logistic regression]] (aka logit, MaxEnt) classifier.
- This class implements regularized [[Logistic regression]] using the ‘liblinear’ library, ‘newton-cg’, ‘sag’, ‘saga’ and ‘lbfgs’ solvers
### \_\_init__:
- `penalty='l2', *, dual=False, tol=0.0001, C=1.0, fit_intercept=True, intercept_scaling=1, class_weight=None, random_state=None, solver='lbfgs', max_iter=100, multi_class='auto', verbose=0, warm_start=False, n_jobs=None, l1_ratio=None`
### Attributes:
- 
### Methods:
- `fit(X, y[, sample_weight])`
	- Fit the model according to the given training data.
- `predict(X)`
	- Predict class labels for samples in X.
