# 🩺 Analysis of a Medical Data Set

## 📘 Project Overview
This project investigates how clinical, demographic, and lifestyle factors influence **medical conditions** and **length of hospital stay**.  
The main goal is to uncover key relationships between patient characteristics and hospital outcomes using Microsoft Excel and Power BI.

---

## 🎯 Research Objectives
The study was guided by the following research questions:

1. **Is there a relationship between age and medical conditions?**  
2. **Does the patient’s medical condition influence the length of hospital stay?**  
3. **Does smoking and alcohol consumption influence medical conditions?**  
4. **Does genetic factors (family history) affect medical conditions?**  
5. **What are the predictors of Length of Stay among patients?**

---

## 🧩 Data Description
The dataset consists of **30,000 patient records** containing demographic, clinical, and lifestyle variables.

| **Category** | **Variables** |
|---------------|---------------|
| **Demographics** | Age, Gender |
| **Clinical Indicators** | Glucose, Blood Pressure, BMI, Oxygen Saturation, Cholesterol, Triglycerides, HbA1c |
| **Lifestyle Factors** | Smoking, Alcohol, Physical Activity, Diet Score, Stress Level, Sleep Hours |
| **Medical History** | Family History, Medical Condition |
| **Outcome Variable** | Length of Stay |

---

## 🧮 Methodology

### **Data Cleaning**
- Conducted in **Microsoft Excel (Power Query)**.  
- Removed irrelevant fields such as *noise* and *random notes*.  
- Reduced decimal places to improve clarity and readability.  
- Converted binary (0/1) values for *Smoking*, *Alcohol*, and *Family History* columns into descriptive labels using the **IF function**.  

### **Data Analysis**
- **Pivot Tables** were used to summarize relationships and patterns.  
- **Charts (Column and Bar)** were used for data visualization.  
- **Regression Analysis** (via Excel’s Data Analysis Toolpak) was conducted to identify predictors of hospital stay.  
- **Power BI** was used for dashboard visualization.

---

## 📊 Analysis and Findings

### **Research Question (a): Is there a relationship between age and medical conditions?**
- **Tool Used:** Pivot Table and Column Chart  
- **Findings:**  
  There is a clear relationship between **age and medical conditions**. Conditions such as **hypertension**, **diabetes**, and **arthritis** were most prevalent among patients aged **50 years and above**.  
- **Insight:**  
  Age is a major determinant of chronic disease occurrence.  
- **Visualization:**  
  Displayed using a **Column Chart** showing the frequency of medical conditions across age groups.

---

### **Research Question (b): Does the patient’s medical condition influence the length of hospital stay?**
- **Tool Used:** Pivot Table and Bar Chart  
- **Findings:**  
  The patient’s **medical condition significantly influences the length of hospital stay**.  
  Patients with chronic illnesses like diabetes and hypertension had **longer hospitalization periods**.  
- **Insight:**  
  Medical condition severity directly affects patient management and hospital resource utilization.  
- **Visualization:**  
  Represented using a **Bar Chart** comparing average hospital stay by condition type.

---

### **Research Question (c): Do smoking and alcohol consumption influence medical conditions?**
- **Tool Used:** Pivot Table and Column Chart  
- **Findings:**  
  There was **no significant relationship** between lifestyle habits (smoking, alcohol) and medical conditions.  
  Interestingly, **non-smokers and non-alcohol users** were more frequently affected by certain diseases.  
- **Insight:**  
  Other variables like stress or genetic predisposition may play stronger roles.  
- **Visualization:**  
  Illustrated using a **Column Chart** comparing medical condition prevalence among smokers vs non-smokers and alcohol users vs non-users.

---

### **Research Question (d): Do genetic factors affect medical conditions?**
- **Tool Used:** Pivot Table and Column Chart  
- **Findings:**  
  **Genetic factors (family history)** influenced several medical conditions except for **hypertension** and **diabetes**.  
- **Insight:**  
  Family history remains important for certain diseases but lifestyle modifications can mitigate genetic risk.  
- **Visualization:**  
  Displayed using a **Column Chart** comparing conditions among patients with and without family history.

---

### **Research Question (e): What are the predictors of Length of Stay among patients?**
- **Tool Used:** Regression Analysis  

#### **Regression Output Summary**

| **Regression Statistics** | **Values** |
|----------------------------|------------|
| Multiple R | 0.4238 |
| R Square | 0.1796 |
| Adjusted R Square | 0.1794 |
| Standard Error | 2.5017 |
| Observations | 30,000 |

#### **ANOVA Table**

| **Source** | **df** | **SS** | **MS** | **F** | **Significance F** |
|-------------|--------|--------|--------|--------|--------------------|
| Regression | 9 | 41087.46 | 4565.27 | 729.47 | 0.0000 |
| Residual | 29,990 | 187687.35 | 6.26 | — | — |
| **Total** | **29,999** | **228774.81** | — | — | — |

#### **Coefficients Table**

| **Variable** | **Coefficient** | **t-Stat** | **P-Value** | **Interpretation** |
|---------------|----------------|-------------|--------------|--------------------|
| Intercept | 11.385 | — | — | Constant value |
| BMI | -0.035 | -12.78 | 2.7E-37 | Small negative effect |
| Oxygen Saturation | -0.070 | -17.66 | 1.86E-69 | Higher oxygen reduces stay |
| Cholesterol | 0.001 | 2.54 | 0.0109 | Slight positive effect |
| Triglycerides | -0.0003 | -1.08 | 0.2803 | Insignificant |
| HbA1c | 0.338 | 28.58 | 2.71E-177 | Strong positive predictor |
| Physical Activity | -0.100 | -11.75 | 8.31E-32 | Higher activity reduces stay |
| Diet Score | -0.171 | -17.99 | 5.92E-72 | Better diet reduces stay |
| Stress Level | 0.238 | 35.57 | 1.9E-271 | Strong positive predictor |
| Sleep Hours | -0.323 | -25.99 | 2.27E-147 | More sleep reduces stay |

#### **Interpretation**
- **Positive Predictors:** Higher **HbA1c** and **Stress Levels** increase the length of hospital stay.  
- **Negative Predictors:** Better **Diet Score**, **Physical Activity**, **Oxygen Saturation**, and **Sleep Hours** reduce length of stay.  
- **Model Fit:**  
  The model explains **17.9% of the variation** in hospital stay (R² = 0.1796).  
  Though moderate, the model highlights meaningful predictors for healthcare improvement.

---

## 🧠 Key Insights
- **Age and chronic conditions** are major determinants of hospital stay.  
- **Healthy lifestyle behaviors** improve recovery and reduce hospital time.  
- **Family history** plays a key role in specific medical conditions.  
- **Regression analysis** highlights HbA1c and stress as major predictors.  

---

## 🧰 Tools & Technologies
- **Microsoft Excel:** Power Query, Pivot Table, Regression, Column & Bar Charts  
- **Power BI:** Data visualization and dashboard creation  

## 🏁 Conclusion
This study reveals that medical outcomes are influenced by a combination of **clinical indicators**, **lifestyle choices**, and **genetic factors**.  
Proactive health management, especially through stress control, diet improvement, and physical activity, can reduce hospital stay duration and improve patient recovery.

---

## 👩‍💻 Author
**Esther Sonnie Egbe**  
*Data Analyst | Healthcare Analytics Enthusiast*  
📧 estyegbe@gmail.com
🔗 [GitHub Profile](https://github.com/Esty-Egbe)



## 🧾 References
- World Health Organization (WHO) – Noncommunicable Diseases Statistics  
- CDC – Hospitalization and Chronic Disease Data  
- Microsoft Excel Data Analysis Toolpak Documentation  
