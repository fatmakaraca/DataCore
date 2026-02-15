# The Impact of Data Sparsity on Recommendation Algorithms

A comparative study of **Memory-Based (User-KNN)** and **Model-Based (SVD)** collaborative filtering under varying sparsity and density levels.

We analyze how recommendation **accuracy (RMSE)**, **diversity**, and **catalog coverage** evolve when data is artificially removed or filtered.  
The project demonstrates robustness differences between neighborhood methods and latent factor models.

📄 Full academic details are available in the paper below.

---

## 📄 Paper
👉 [Read the Paper (PDF)](paper/paper.pdf)

---

## 🚩 Research Questions
- Which approach is more resilient to extreme sparsity?
- When does diversity become random noise?
- What is the trade-off between accuracy and long-tail exposure?

---

## 🧠 Methods

**Memory-Based:**  
- User-Based KNN  
- Pearson similarity  

**Model-Based:**  
- Matrix Factorization  
- SVD with Gradient Descent  
- Latent feature learning  

---

## 🧪 Experimental Design

**Sparsity Injection:** remove 20%, 40%, 60%, 80% of interactions (MCAR).  
**Density Filtering:** iterative K-core pruning to create cleaner matrices.

---

## 📊 Metrics
- RMSE  
- Diversity  
- Coverage  

---

## 🗂 Dataset
MovieLens 1M  
6,040 users · 3,706 movies · ~1M ratings · ~95% sparse

---

## 🏆 Main Outcomes
- SVD preserves stable performance under heavy sparsity.  
- KNN rapidly loses reliability as overlap disappears.  
- High apparent diversity in sparse regimes may indicate noise.  
- Optimizing purely for accuracy reduces catalog exploration.

---

---

## ⚙️ Installation

Clone the repository 

```bash
git clone https://github.com/fatmakaraca/DataCore
```

### 👥 Authors

Öykü Tuğyan
Fatma Karaca
Ebrar Pınar Kuz


