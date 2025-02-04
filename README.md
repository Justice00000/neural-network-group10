# Classification Project for Group 10

##  Project Overview
This project aims to **predict water potability** based on various properties using machine learning models. The dataset consists of water quality parameters, and the goal is to develop models that effectively classify whether a given water sample is **potable (safe to drink) or not**.

## Video Presentation 

Link: https://drive.google.com/file/d/1N9TZa7hTzWw-FE-8IbPJxU3zUaI6UJyU/view?usp=sharing



## Models Implemented
We trained and evaluated **two different models**, each utilizing different **regularization techniques** and **optimizers** to compare performance:

1️⃣ **L1 Regularization with RMSprop Optimizer (Justice's Model)**  
2️⃣ **L2 Regularization with Adam Optimizer (Madol Abraham Kuol Madol's Model)**  
2️⃣ **L2 Regularization with SGD Optimizer (Willy Kalisa's Model)** 

Both models are assessed based on **accuracy, precision, recall, F1-score, and loss curves**.

---

## Table of Model Comparisons

| Team Member                  | Regularizer        | Optimizer | Early Stopping | Dropout Rate | Accuracy | F1 Score | Recall | Precision |
|------------------------------|-------------------|-----------|----------------|--------------|----------|----------|--------|-----------|
| Willy Kalisa                 | L2 Regularization | SGD       | Yes            | 0.6931       | 0.4345   | 0.3021   | 0.7733 | N/A       |
| Madol Abraham Kuol Madol     | L2 Regularization | Adam      | Yes            | N/A          | 0.729     | 0.479     | 0.33    | 0.71       |
| Justice Chukwuonye           | L1 Regularization | RMSprop   | Patience=10, monitor='val_loss'            | 0.3, 0.2     | 0.62     | 0.77     | 1.00   | 0.62      |

--- 


---

## Performance Analysis
Willy Kalisa's model, using L2 regularization and SGD, achieves 43.45% accuracy with high recall (77.33%) but low precision. The high dropout rate (0.6931) may have impacted performance.

Madol Abraham Kuol Madol's model, with L2 regularization and Adam optimizer, performs better with 72.90% accuracy, 71.00% precision, and 47.90% F1 score, though recall is lower (33.00%).

Justice Chukwuonye's model, using L1 regularization and RMSprop, achieves 62.00% accuracy with an excellent F1 score (77.00%) and perfect recall (100.00%), but lower precision (62.00%).

Overall, each model has trade-offs. Fine-tuning dropout and regularization could further optimize performance.

---




---

## How to Run the Project
To set up and run this project locally:

### **1️⃣ Install Dependencies**
Ensure you have **Python 3.9+** installed, then run:
```bash
pip install tensorflow
```
### **2️⃣ Run the Training Notebooks**
Navigate to the notebooks folder and open the notebooks in the different branches 

### **3️⃣ Evaluate the Models**
Run all cells in the notebooks.
View loss curves, accuracy metrics, and confusion matrices.


## Contributors
- Justice Chukwuonye (CeeJay): Trained L1 + RMSprop.
- Madol Abraham Kuol Madol: Training L2 + Adam model.
- Willy Kalisa: Training L2 + SGD Model
- Instructor: Providing feedback and project guidelines.
