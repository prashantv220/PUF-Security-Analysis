# ML-PUF Security Analysis

**Analysis of Multi-Level Arbiter PUFs (ML-PUFs) using linear models, achieving up to 97% accuracy, and delay recovery in Arbiter PUFs via constrained optimization.**

---

## 📌 Overview
- **Multi-Level PUF Analysis**  
  Designed a **64-dimensional feature map** (via Khatri-Rao product) and trained linear classifiers on **6.4K train / 1.6K test CRPs**, achieving **97% accuracy** with Logistic Regression and outperforming Linear SVM (~93%).  

- **Delay Recovery in Arbiter PUFs**  
  Formulated and solved a **65×256 constrained least-squares optimization** problem to recover valid **non-negative delay parameters** from underdetermined models.  

- **Comparative Experiments**  
  Evaluated Logistic Regression vs Linear SVM, analyzing the effect of hyperparameters (**C, penalty, tolerance**) on accuracy.  

---

## 🔑 Key Results
- Logistic Regression (L2, C=140): **97% accuracy**  
- Linear SVM (L2, C=100): **~93% accuracy**  
- Delay recovery method reconstructs consistent delay vectors from linear model coefficients.  

---

## 🛠 Tech Stack
- **Python 3**  
- **NumPy**  
- **scikit-learn** (`LogisticRegression`, `LinearSVC`)  
- **SciPy** (Khatri-Rao product)  

---
