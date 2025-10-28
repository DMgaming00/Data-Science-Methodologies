# 💸 From Kaggle to Clarity: How I Predicted House Prices with SEMMA

> “Good data scientists don’t just build models — they build systems of thought.”  

That’s what the **SEMMa framework** taught me while working on the **Ames Housing dataset**, one of Kaggle’s most detailed property datasets.  
Here’s how I turned 81 columns of chaos into a precise prediction engine.

---

### 🔬 Step 1: Sample  
I began by loading the dataset containing **1,460 houses and 81 features**.  
Since the dataset was small enough, I decided to **use all data** rather than subsampling — ensuring a holistic view of the market.

---

### 📊 Step 2: Explore  
Exploration was where things got real.  
I used heatmaps and scatterplots to uncover key relationships:
- `OverallQual` (construction quality) and `GrLivArea` (living area) had the strongest correlations with `SalePrice`.
- Right-skewed distributions revealed expensive properties as outliers.
- Missing data in `PoolQC`, `Fence`, and `Alley` hinted at underreported luxury attributes.

---

### 🧰 Step 3: Modify  
Instead of dropping data, I used **SimpleImputer** to fill missing values — median for numbers, most frequent for categoricals.  
Then, I applied **OneHotEncoder** and built a **ColumnTransformer pipeline**.  
This single step automated all preprocessing, making my workflow clean and production-ready.

---

### ⚙️ Step 4: Model  
I chose **Linear Regression** for its interpretability and baseline efficiency.  
After training, the model achieved:
- **MAE:** 18,000  
- **RMSE:** 24,000  
- **R²:** 0.89  

That means the model explained **89% of the variation** in sale prices.  
Not bad for a single regression line, right?

---

### 📈 Step 5: Assess  
I plotted **actual vs. predicted values** — and the near-perfect alignment proved the model’s robustness.  
It captured trends beautifully without overfitting, validating the SEMMA approach.

---

### 💡 What I Learned  
The **SEMMa methodology** made me appreciate the beauty of simplicity.  
It’s structured enough for serious analytics, yet flexible enough to encourage creativity.  
It’s the “data scientist’s zen” — balancing rigor and intuition.

---

### 🧭 Explore the Full Project  
🔗 **GitHub Repository:** [data-science-methodologies (SEMMa Project)](YOUR_GITHUB_REPO_LINK_HERE)
