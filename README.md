# Assignment 2 – Summary

This assignment explores three major areas of digital engineering:  
**GPS positioning**, **machine learning**, and **deep learning**.  
Each part includes implementation, evaluation, and result interpretation.

---

## Part 1 – Non-linear Estimation (LSE & Gradient Descent)

This section estimates a GPS receiver’s 3D position and clock offset using:

- **Non-linear Least Squares (LSE)**
- **Gradient Descent optimization**

### What Was Done
- Loaded pseudorange and satellite position files  
- Added measurement noise  
- Implemented Euclidean distance and iterative LSE  
- Computed corrections, covariance matrix, APV  
- Implemented gradient descent with cost and gradient functions  
- Tuned learning rates and compared convergence  
- Visualized misclosure, corrections, and position error per iteration  

### Key Results
- LSE converged in **5 iterations**, very efficient  
- Gradient Descent required **739+ iterations**  
- Too-small learning rates slowed convergence  
- Final 3D position error ≈ **5.4 m**  
- LSE produced more stable covariance & APV measures  

---

## Part 2 – Student Depression Prediction (Logistic Regression)

This section builds a binary classification model on a student depression dataset.

### What Was Done
- Cleaned data: removed missing & duplicate values, encoded categorical features  
- Created three datasets:
  - Full dataset  
  - First-two-feature subset  
  - 3% small dataset  
- Trained Logistic Regression for all cases  
- Calculated training/testing accuracy & log loss  
- Visualized confusion matrix and classification report  
- Compared with **Naive Bayes** and **KNN**  
- Answered seven analysis questions  

### Key Results
- Full dataset achieved best accuracy (**~0.85**)  
- Only two features → **underfitting**  
- Small dataset → **mild overfitting**  
- Dataset is imbalanced but manageable  
- Logistic Regression outperformed Naive Bayes and KNN  
- Recall is more important than precision for detecting depression  

---

## Part 3 – MNIST Digit Classification (MLP vs CNN)

This section compares two neural network models using the MNIST handwritten digit dataset.

### What Was Done
- Loaded MNIST CSV data (train & test)  
- Reshaped samples into 28×28 images  
- Visualized random digits  
- Preprocessed and normalized pixel values  
- Built and trained:
  - **MLP model**  
  - **CNN model**  
- Evaluated both using confusion matrix & classification report  

### Key Results
- CNN achieved significantly higher accuracy  
- MLP struggled due to lack of spatial feature learning  
- CNN generalized better with fewer parameters and higher efficiency  

---

## Conclusion
Assignment 2 demonstrates competency in:

- **GPS position estimation and optimization (Part 1)**  
- **Machine learning model development and evaluation (Part 2)**  
- **Deep learning image classification (Part 3)**  

The work highlights the strengths of each method and explains model behavior through visualization, error analysis, and performance comparison.
