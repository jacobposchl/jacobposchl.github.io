---
title: "Self-Study"
permalink: /self-study/
layout: single
---

This is where I post what I've learned for the week.

### Week of May 26, 2025
**Vector–Jacobian Product**  
*I learned the geometric interpretation of the vector–Jacobian product and why it’s central to efficient backpropagation. I visualized the Jacobian as a hilly landscape and the gradient as gravity, then introduced the vector as “wind” that redirects the path toward minima. Experimented with a small PyTorch demo to compute vector–Jacobian products manually, and I’ll build an interactive visualization next.*

---

### Week of May 12, 2025
**Data Types and Missing Values (Pandas)**  
*Explored how Pandas categorizes data types and methods for handling nulls. Practiced `fillna`, `dropna`, and type-casting strategies. Documented a workflow for cleaning a messy real-world dataset, including performance considerations when converting large columns.*

**Grouping and Sorting (Pandas)**  
*Used `groupby` to compute complex aggregates and custom transformations. Combined multi-level sorting with custom key functions. Applied these techniques to an EDA of sales data, uncovering group-specific trends.*

**Summary Functions and Maps (Pandas)**  
*Worked with `.agg()`, `.transform()`, and `.apply()` to summarize and reshape DataFrames. Learned when to prefer vectorized map functions versus row-wise `apply`. Built a small library of mapping utilities for categorical encoding.*

**Indexing, Selecting, Assigning (Pandas)**  
*Drilled into `.loc`, `.iloc`, boolean masks, and their pitfalls around views vs. copies. Wrote helper functions for dynamic column selection and assignment that I’ll reuse in data pipelines.*

**Project Reflection**  
*Consolidated the month’s Pandas study into a Colab notebook, linking each concept to downstream ML preprocessing steps. Packaged snippets into a reusable template for future pipeline work.*

---

### Week of April 28, 2025
**Build Classifier for Any Dataset (Titanic, MNIST)**  
*Developed end-to-end pipelines: data cleaning, feature engineering, model training, and evaluation. Tuned hyperparameters with grid search and inspected model diagnostics. Documented differences between tabular (Titanic) and image (MNIST) workflows.*

**Model Evaluation Metrics**  
*Dove deep into precision, recall, F1-score, ROC/AUC, and confusion matrices. Wrote custom metric functions and plotted precision-recall curves to understand trade-offs in imbalanced settings.*

**KNN & Decision Trees**  
*Experimented with K-Nearest Neighbors and Decision Tree classifiers on UCI datasets. Visualized decision boundaries and learned how hyperparameters (e.g., `k`, tree depth) influence overfitting.*

**Linear & Logistic Regression**  
*Implemented both models from scratch using NumPy. Compared analytical solutions to gradient descent. Added L2 regularization and plotted learning curves to understand under- and over-fitting behavior.*

**Renaming & Combining (Pandas)**  
*Mastered `merge`, `join`, and `concat` for combining datasets. Cleaned inconsistent column names and standardized schemas across multiple CSVs. Demonstrated best practices for reproducible data merges.*

---

### Week of April 7, 2025
**CNN for Image Classification (CIFAR-10)**  
*Built a convolutional network in PyTorch: conv→ReLU→pool stacks followed by fully connected layers. Trained on CIFAR-10, tuned learning rates, and added batch normalization. Analyzed misclassifications via confusion matrices.*

**Unsupervised Learning Project**  
*Completed a mini-project combining PCA and KMeans on handwritten digit data. Visualized clusters in reduced dimensions and measured cluster purity against labels.*

**KMeans & PCA**  
*Studied the math behind PCA eigen decomposition and KMeans cluster centroids. Ran experiments varying `n_components` and `k`, then plotted explained variance to choose optimal dimensionality.*

**MLP Classifier (MNIST)**  
*Trained a multilayer perceptron on MNIST with one hidden layer. Added dropout and tested different optimizers. Tracked train/validation loss curves to diagnose overfitting.*

**SVMs & Ensemble Models**  
*Applied Support Vector Machines and ensemble methods (Random Forest, AdaBoost) to multiple datasets. Compared performance, ran grid searches, and documented when each method excels.*

---

### Week of March 24, 2025
**Autograd: requires_grad, .backward(), Gradients**  
*Explored PyTorch’s automatic differentiation internals. Manually toggled `requires_grad`, traced gradient flow through a tiny network, and visualized computation graphs to solidify how backward passes propagate.*

**torch.Tensor Basics**  
*Practiced tensor creation, reshaping, broadcasting, and memory views. Compared tensor operations to NumPy arrays, then integrated tensor computations into simple neural layers.*

**Intermediate ML (Kaggle)**  
*Worked through Kaggle tutorials on Titanic and Housing. Focused on feature engineering, cross-validation, and stacking models. Documented pipeline design for reproducible competitions.*

**GAN (MNIST Digit Generator)**  
*Built a basic Generative Adversarial Network in PyTorch. Trained on MNIST, watched generator and discriminator loss interplay, and saved epoch-wise image grids to track generation quality.*

**LSTM for Sequence Data**  
*Implemented a unidirectional LSTM for synthetic sequence classification. Visualized hidden and cell states over time and compared sequence-to-one vs. sequence-to-sequence setups.*
