# 🧠 How I Used the CRISP-DM Framework to Predict Titanic Survivors (and What It Taught Me About Human Data)

> *“What if we could have predicted who survived the Titanic tragedy — not with luck, but with data?”*  
That’s the question I set out to answer with the **CRISP-DM (Cross Industry Standard Process for Data Mining)** methodology.  

---

### 🚢 The Story Behind the Dataset
The **Titanic dataset** is a timeless benchmark in data science. It’s not just about numbers — it’s a story about survival, inequality, and human behavior under pressure.  

I wanted to explore this dataset from a **data mining perspective**, applying the **CRISP-DM framework** to go beyond modeling accuracy and extract genuine, human insights.

---

### ⚙️ Step 1: Business Understanding  
Before coding, I defined the goal — **predict survival** based on personal and ticket details.  
The bigger question, however, was *why certain people survived more than others*. Was it gender? Wealth? Age? Or sheer luck?

This is the “why” CRISP-DM forces us to ask first — turning curiosity into a concrete analytical question.

---

### 🔍 Step 2: Data Understanding  
I explored 891 records of passengers, each with 12 features.  
Using pandas and visualization, I noticed patterns:
- Women had a **74% survival rate**, while men had just **19%**.
- **First-class** passengers had much higher chances of survival.
- **Age** and **Fare** revealed subtle social hierarchies aboard the ship.

Visualizing this data made one thing clear — social and economic class *literally* determined life or death.

---

### 🧹 Step 3: Data Preparation  
I handled missing values methodically:
- Filled `Age` with the median.
- Replaced missing `Embarked` values with the mode.
- Dropped the sparsely populated `Cabin` column.  

I also engineered new features like `FamilySize = SibSp + Parch + 1`, revealing that passengers traveling with families had higher odds of survival.

---

### 🤖 Step 4: Modeling  
I built a **Random Forest Classifier** using scikit-learn pipelines — ensuring each preprocessing step (encoding, imputation, scaling) was automated.  

The model achieved **83% accuracy**, and feature importance analysis showed:
- `Sex`
- `Pclass`
- `Fare`
- `Age`  
as the top survival predictors.

---

### 📈 Step 5: Evaluation  
Precision, recall, and F1-score metrics confirmed balanced performance.  
The **feature importance chart** told a deeper story: gender and wealth were survival’s biggest allies.

---

### 🚀 Step 6: Deployment  
Finally, I serialized the pipeline using **Joblib**, making it reusable for new predictions — a fully deployable end-to-end CRISP-DM project.

---

### 💡 What I Learned
CRISP-DM reminded me that **data science is storytelling with discipline**.  
It forces structure without killing creativity.  
And in this case, it helped uncover how data can reflect society — even in tragedy.

---

### 🧭 Explore the Full Project  
🔗 **GitHub Repository:** [data-science-methodologies (CRISP-DM Project)](https://github.com/DMgaming00/Data-Science-Methodologies)
