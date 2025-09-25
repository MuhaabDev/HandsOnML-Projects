# 🏠 Chapter 2 – End-to-End Machine Learning Project  

This notebook is based on **Hands-On Machine Learning (3rd Edition), Chapter 2**.  
The goal of this project is to walk through a complete **end-to-end ML workflow** using the **California Housing dataset**.  

---

## 📚 Steps in the Notebook  

### 1. Import Libraries  
- `numpy`, `pandas` → data handling  
- `matplotlib`, `seaborn` → visualization  
- `scikit-learn` → preprocessing, pipelines, models, and evaluation  

### 2. Load & Explore the Data  
- Dataset: **California Housing Prices**  
- Visualized distributions (histograms) and geographic scatter plots  
- Learned to spot patterns and correlations (e.g., **median income** is the strongest predictor of house value)  
- Compared **random train/test split** vs **stratified sampling** (based on income categories)  

### 3. Prepare the Data for ML  
- **Separate predictors & labels** (`housing` vs `median_house_value`)  
- **Handle missing values**:  
  - SimpleImputer  
  - KNNImputer  
  - IterativeImputer  
- **Categorical attributes**: encoding via `OneHotEncoder`  
- **Feature scaling & transformation**:  
  - Min-Max scaling  
  - Standardization  
  - Bucketizing (binning income categories)  
- Learned about **multi-feature transformations** (e.g., combining latitude & longitude)  
- Applied **target transformation** when labels are skewed  

### 4. Pipelines  
- Built **custom transformers**  
- Used **Scikit-Learn Pipelines** to streamline preprocessing + modeling  
- Learned why pipelines are critical for **clean, reproducible, and production-ready ML workflows**  

### 5. Model Training & Evaluation  
- Trained **Linear Regression**, **Decision Tree**, and **Random Forest**  
- Compared models with **RMSE** (Root Mean Squared Error) vs **MAE** (chose RMSE since it penalizes larger errors more strongly)  
- Applied **cross-validation** for reliable performance estimation  

### 6. Fine-Tuning the Model  
- **GridSearchCV** vs **RandomizedSearchCV** → understood the trade-offs  
- Tuned hyperparameters of the Random Forest model  
- Selected the best estimator based on CV results  

---

## 📖 Key Learnings  
- ✅ How to **look at the big picture** before modeling  
- ✅ Difference between **random sampling vs stratified sampling**  
- ✅ Why **RMSE > MAE** in this case  
- ✅ How to **explore correlations** & interpret scatter plots  
- ✅ How to **prepare data properly**: imputers, encoders, scaling  
- ✅ What **pipelines** are and why they matter in production ML  
- ✅ How to **fine-tune models** and avoid overfitting  
- ✅ Learned that ML is not just training a model — it’s about building a **full reproducible workflow**  

---

## ⚙️ Requirements  
Install the dependencies before running the notebook:  

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
````

---

## 🚀 How to Run

Clone the repository:

```bash
git clone https://github.com/USERNAME/HandsOnML-Projects.git
cd HandsOnML-Projects/chapter2
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Open the notebook:

```bash
jupyter notebook chapter2.ipynb
```

---

## 📊 Results

* The final model was a **Random Forest Regressor** with hyperparameter tuning.
* Achieved an RMSE around **X** (fill in once you run your tuned model).
* Learned how model choice + data preprocessing dramatically affect performance.

---
