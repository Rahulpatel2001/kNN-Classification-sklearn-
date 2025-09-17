RAHUL KUDURU 700763240
# kNN Classification on Iris Dataset (sklearn)

## Project Overview
This project demonstrates **k-Nearest Neighbors (kNN)** classification on the **Iris dataset** using only two features:  
- Sepal Length  
- Sepal Width  

We train kNN classifiers with different values of `k = 1, 3, 5, 10` and visualize the **decision boundaries**.  
The goal is to understand how the parameter `k` affects the complexity of the decision boundary and model generalization.

---

##  Technologies Used
- Python 3
- scikit-learn
- matplotlib
- numpy

---

## Steps Performed
1. Loaded the Iris dataset from `sklearn.datasets`.
2. Selected only two features: **sepal length** and **sepal width**.
3. Trained `KNeighborsClassifier` with `k = 1, 3, 5, 10`.
4. Plotted the **decision boundaries** for each value of k.
5. Discussed how the boundaries change as k increases.

---

## Results & Observations
- **k = 1** → Very jagged, irregular boundaries. Overfits to noise (high variance, low bias).  
- **k = 3** → Smoother boundaries, good balance between flexibility and generalization.  
- **k = 5** → Even smoother, stable patterns emerge, slightly higher bias.  
- **k = 10** → Very smooth, loses fine details (risk of underfitting).  

👉 In summary:
- **Small k** → Complex boundaries (overfitting).  
- **Large k** → Smooth/simple boundaries (underfitting).  
- **Moderate k (3–5)** → Best trade-off between bias and variance.  
