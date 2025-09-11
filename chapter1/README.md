# Chapter 1 – Satisfaction vs GDP

This notebook is based on **Hands-On Machine Learning (3rd Edition)**, Chapter 1.  
The goal is to explore the relationship between a country’s GDP per capita and the average life satisfaction of its citizens.

---

## 📚 Steps in the Notebook

1. **Import Libraries**
   - `matplotlib` for visualization
   - `pandas` for data handling
   - `scikit-learn` (`LinearRegression`) for modeling

2. **Download and Prepare the Data**
   - Dataset: [lifesat.csv](https://github.com/ageron/data/raw/main/lifesat/lifesat.csv)
   - Extract GDP per capita (`X`) and Life satisfaction (`y`).

3. **Visualize the Data**
   - Scatter plot of GDP per capita vs. life satisfaction.

4. **Select and Train a Linear Model**
   - Use `LinearRegression` from scikit-learn.
   - Fit the model to the data.

5. **Make a Prediction**
   - Predict life satisfaction for Cyprus (GDP per capita ≈ 37,655 in 2020).
   - Output: `[[6.30]]`

---

## 📈 Visualization
The scatter plot shows a positive correlation between GDP per capita and life satisfaction.

---

## ⚙️ Requirements
Install the dependencies before running the notebook:

```bash
pip install matplotlib pandas scikit-learn
````

---

## 🚀 How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/USERNAME/HandsOnMl3rdEdition.git
   cd HandsOnMl3rdEdition/chapter1
   ```
2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```
3. Open the notebook:

   ```bash
   jupyter notebook SatisfactoinVsGDP.ipynb
   ```

---
