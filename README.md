# SVM_on_NonlinearDataset
ELE489-Fundamentals of Machine Learning HW5

# 🌙 SVM Classification on Moons Dataset

This project demonstrates the use of **Linear SVM** and **Non-linear SVM (RBF kernel)** to classify a synthetic 2D the *"moons"* dataset.


# 📌 Project Summary

Exploring how linear and non-linear Support Vector Machines (SVMs) behave on a non-linearly separable dataset. This includes:

- Generating the moons dataset
- Training a linear SVM and visualizing its limitations
- Training an RBF SVM and visualizing its decision surface in 2D and 3D
- Explaining why linear SVM fails and RBF SVM succeeds
  

# 📊 Dataset

- **Type**: Synthetic
- **Source**: `sklearn.datasets.make_moons`
- **Samples**: 400
- **Noise**: 0.2
- 

##  Models Used

### 1. Linear SVM
- `kernel='linear'`
- Shows poor performance on this dataset due to the 'S' shaped decision boundary needed which is nonlinear

### 2. Non-linear SVM (RBF Kernel)
- `kernel='rbf'`
- Successfully separates the classes with a flexible, curved boundary


## 📈 Visualizations

###  Linear SVM
- 2D scatter plot with decision boundary and margins
- Support vectors highlighted

###  RBF SVM
- 2D plot with curved decision boundary and ±1 margins
- 3D plot showing the decision surface


##  Example Outputs

### Linear SVM

- Accuracy: ~80–85%
- Misclassified points: many
- Margin: constant (2/‖w‖)
- Poor separation

### RBF SVM

- Accuracy: ~95–100%
- Smooth curved boundary
- Margin: varies across space
- Support vectors optimized on boundary
