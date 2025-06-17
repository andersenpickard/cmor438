## Perceptron Classification: Breast Cancer Dataset

This project implements and analyzes the Perceptron algorithm applied to the breast cancer dataset from sklearn.

## What is Perceptron?

Perceptron is a simple classification algorithm. It builds a linear decision boundary separating two features by updating weights based on prediction errors. The boundary should be interpreted as a firm threshold between the two features.

The perceptron model is defined as:


Weights 
w
 and bias 
b
 are updated through the perceptron learning rule each time the model misclassifies a training example.

The perceptron works best on linearly separable datasets and does not produce probabilistic outputs. It is a deterministic, mistake-driven learner that converges only if a perfect linear separator exists.

In this project, we use the Perceptron to classify whether an MLB player is an All-Star or not, based on Statcast features such as exit velocity, barrel percentage, and launch angle.


## Dataset

I am using the Breast Cancer Wisconsin dataset available in `sklearn.datasets`. This dataset contains 569 observations with 30 numerical features and a binary target (malignant or benign).

## Perceptron Model

- Written using NumPy, based off the implementation in our course module
- Trains with manually adjusted/defined learning rate and epoch count
- Visualizes decision boundaries and learning curves

## Exploration

- First attempt uses the features `worst perimeter` and `worst area` 
- Second attempt uses the features `worst concavity` and `worst symmetry` 
