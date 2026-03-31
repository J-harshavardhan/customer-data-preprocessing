# 🧹 Customer Data Preprocessing

A Jupyter Notebook demonstrating core data preprocessing techniques applied to a synthetic customer dataset — a mandatory step before training any ML model.

---

## 📁 Files

| File | Description |
|---|---|
| `preprocessing.ipynb` | Main notebook with all tasks, markdown explanations, and code |
| `README.md` | This file |

---

## 🧪 Tasks Covered

### Task 1 — Data Cleaning
- Impute missing `age` values with the **median**
- Impute missing `city` values with the **mode**
- Remove **duplicate rows**

### Task 2 — Categorical Encoding
- **One-Hot Encoding** on `city` → creates binary columns per city
- **Label Encoding** on `gender` → maps Female=0, Male=1

### Task 3 — Feature Scaling
- **Min-Max Scaling** → compresses values to [0, 1]
- **Standardisation** → transforms to mean=0, std=1

---

## ⚙️ Setup & Run

```bash
# Install dependencies
pip install pandas numpy scikit-learn jupyter

# Launch the notebook
jupyter notebook preprocessing.ipynb
```

---

## 💡 Key Takeaway: MinMax vs StandardScaler

| Use Case | Recommended |
|---|---|
| Neural networks, image data | MinMaxScaler |
| Data with outliers | StandardScaler |
| SVM, PCA, Logistic Regression | StandardScaler |
| KNN, K-Means | MinMaxScaler |

---

## 🚀 How to Push to GitHub

```bash
git init
git add preprocessing.ipynb README.md
git commit -m "Add data preprocessing assignment"
git branch -M main
git remote add origin https://github.com/J-harshavardhan/customer-data-preprocessing
git push -u origin main
```
