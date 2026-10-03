# Comparative Study of Gradient Descent Optimization Techniques for Linear Regression

## 📌 Project Overview

This project is a practical implementation and comparative study of different **Gradient Descent optimization techniques** using a simple **Linear Regression** model.

The primary objective of this project is not to build a complex machine learning model, but to understand **how different optimization algorithms learn and update model parameters**.

The same Linear Regression model is trained using multiple optimization approaches, and their convergence behavior and final loss are compared.

---

## 🎯 Objectives

The main objectives of this project are to:

- Understand Gradient Descent practically.
- Implement optimization algorithms from scratch using Python and NumPy.
- Understand how gradients are calculated and used to update model parameters.
- Compare different Gradient Descent optimization techniques.
- Study the effect of learning rate and momentum on optimization.
- Visualize loss reduction during training.
- Compare the convergence behavior of different optimizers.
- Understand how optimization affects the training of a machine learning model.

---

## 📚 Learning Reference

This project was developed after studying and referring to the Medium article:

### *Gradient Descent from Scratch in Python: A Complete Beginner’s Guide*

**Author:** Sourav Mukherjee  
**Published on:** Medium / Bongquisitive Tech  
**Published:** July 21, 2026

🔗 **Original article:**  
https://medium.com/bongquisitive-tech/gradient-descent-from-scratch-in-python-a-complete-beginners-guide-09a2339a5a41

👤 **Author:**  
Sourav Mukherjee  
https://medium.com/@sourav15

The article provided the conceptual foundation for understanding Gradient Descent, including the ideas of loss functions, gradients, parameter updates, learning rates, Stochastic Gradient Descent, and Momentum.

The project in this repository extends that learning into a practical comparative experiment using a Linear Regression model.

> **Note:** The referenced article was used as a learning resource and conceptual reference. The implementation and experimental comparison in this project were developed as a practical exercise based on those concepts.

---

## 🧠 Concepts Covered

### 1. Linear Regression

The project uses a simple Linear Regression model:

\[
\hat{y} = wx + b
\]

Where:

- `w` = weight
- `x` = input feature
- `b` = bias
- `ŷ` = predicted output

---

### 2. Mean Squared Error

Mean Squared Error (MSE) is used as the loss function.

\[
MSE = \frac{1}{n}\sum_{i=1}^{n}(y_i-\hat{y}_i)^2
\]

The objective of optimization is to minimize this loss.

---

### 3. Gradient Calculation

The gradients of the loss with respect to the model parameters are calculated manually.

For the weight:

\[
\frac{\partial MSE}{\partial w}
=
\frac{2}{n}\sum x_i(\hat{y}_i-y_i)
\]

For the bias:

\[
\frac{\partial MSE}{\partial b}
=
\frac{2}{n}\sum(\hat{y}_i-y_i)
\]

These gradients determine how the parameters should be adjusted.

---

## ⚙️ Optimization Algorithms Implemented

The same Linear Regression model is trained using the following optimization techniques:

### 1. Batch Gradient Descent

The entire dataset is used to calculate the gradient before each parameter update.

### 2. Stochastic Gradient Descent

One training sample is used at a time to calculate the gradient and update the parameters.

### 3. Mini-Batch Gradient Descent

A small group of training samples is used for each parameter update.

### 4. Momentum Gradient Descent

Momentum incorporates information from previous updates to influence the current update.

### 5. Momentum with Learning-Rate Decay

Momentum is combined with a gradually decreasing learning rate.

---

## 📊 Dataset

A simple educational dataset is used for the experiment.

### Problem

Predict a student's **Exam Score** based on their **Study Hours**.

| Study Hours | Exam Score |
|-------------|------------|
| 1 | 35 |
| 2 | 42 |
| 3 | 48 |
| 4 | 55 |
| 5 | 61 |
| 6 | 68 |
| 7 | 73 |
| 8 | 81 |
| 9 | 86 |
| 10 | 92 |

The dataset is intentionally simple so that the focus remains on understanding and comparing optimization algorithms rather than dataset complexity.

---

## 🛠️ Technologies Used

- **Python**
- **NumPy**
- **Pandas**
- **Matplotlib**
- **Jupyter Notebook**

No high-level machine learning library is used to perform the actual model training.

The optimization algorithms are implemented manually to make the parameter-update process explicit and easier to understand.

---

## 📁 Project Structure

```text
optimization-linear-regression/
│
├── optimization_linear_regression.ipynb
│
└── README.md
```

---

## 🔬 Experimental Workflow

The project follows this workflow:

```text
Dataset
   ↓
Linear Regression Model
   ↓
Prediction
   ↓
MSE Loss
   ↓
Gradient Calculation
   ↓
Optimization Algorithm
   ↓
Parameter Update
   ↓
Loss Tracking
   ↓
Optimizer Comparison
```

---

## 📈 Evaluation and Comparison

The optimization algorithms are compared using:

- Final Mean Squared Error
- Loss reduction over epochs
- Convergence behavior
- Training stability
- Learned weight
- Learned bias

Loss curves are plotted to visualize how each optimizer approaches a lower-error solution.

---

## 📊 Visualizations

The notebook includes visualizations for:

### Dataset

Study Hours vs Exam Score.

### Loss Curves

Comparison of loss reduction for different optimization algorithms.

### Log-Scale Loss Curves

A logarithmic loss plot is used to make differences in convergence behavior easier to observe.

### Regression Lines

The regression lines generated by the different optimization approaches are compared against the original data.

### Final MSE

A comparison of the final MSE obtained by each optimizer.

---

## 💡 Key Learning Outcomes

Through this project, I gained practical understanding of:

- How a Linear Regression model makes predictions.
- How a loss function measures prediction error.
- How gradients indicate the direction of parameter adjustment.
- How Gradient Descent updates model parameters.
- The difference between Batch GD, SGD, and Mini-Batch GD.
- How Momentum affects optimization.
- How learning-rate decay changes the optimization process.
- How optimization choices influence convergence.
- How to implement optimization algorithms without relying on high-level ML libraries.

---

## 🔎 Why Linear Regression?

Linear Regression was intentionally selected as the model for this project.

A more complex model such as a neural network could make the project harder to interpret because the focus would shift toward model architecture and backpropagation.

By keeping the model simple, the project focuses primarily on:

> **How different optimization algorithms learn the model parameters.**

This makes it easier to observe and compare the behavior of each optimization technique.

---

## 📌 Project Focus

The central question of this project is:

> **How does the choice of optimization algorithm affect the training and convergence of the same Linear Regression model?**

Instead of changing the model architecture, the experiment keeps the model constant and changes the optimization method.

This provides a clearer way to study optimization.

---

## 🚀 Possible Future Improvements

The project can be extended by:

- Testing different learning rates.
- Testing different momentum values.
- Experimenting with different mini-batch sizes.
- Adding more features to the dataset.
- Using a larger real-world dataset.
- Comparing optimization algorithms on a more complex regression problem.
- Extending the implementation to Logistic Regression.
- Implementing optimization for a simple neural network.
- Comparing the from-scratch implementation with library-based implementations.

---

## 📖 Reference

**Mukherjee, Sourav.**  
*"Gradient Descent from Scratch in Python: A Complete Beginner’s Guide."*  
Bongquisitive Tech, Medium, July 21, 2026.

Original article:

https://medium.com/bongquisitive-tech/gradient-descent-from-scratch-in-python-a-complete-beginners-guide-09a2339a5a41

Author:

https://medium.com/@sourav15

The article was referred to for learning the fundamental concepts and implementation ideas behind Gradient Descent, including loss functions, gradients, learning rates, SGD, and Momentum.

---

## 👩‍💻 Author

**Sneha C. R.**

This project was created as a practical learning project to strengthen my understanding of **Machine Learning Optimization Algorithms and Gradient Descent**.