# Traffic Accident Severity Prediction in the UK  

## 📌 Overview  
Traffic accidents are a significant global concern, ranking among the leading causes of injuries and fatalities (Chand et al., 2021). According to the **WHO (2020)**, approximately **1.35 million people die annually**, and **20–50 million people suffer nonfatal injuries** due to traffic accidents. By 2030, traffic accidents are projected to become the **fifth leading cause of death worldwide** (Sameen et al., 2017).  

Because of the uncertainty and randomness inherent in traffic accidents, **predicting accident severity** and **analyzing the key influencing factors** have become critical research directions. Researchers have increasingly adopted **machine learning (ML) techniques**, as they allow for flexible modeling of multidimensional data to forecast traffic accident outcomes (Lord et al., 2010).  

This project applies **machine learning methods** to predict the severity of traffic accidents in the UK, aiming to:  
- Identify the **key influencing factors** contributing to accident severity.  
- Compare the **performance of different ML models** in predicting accident severity.  
- Provide insights that may support **traffic safety policies and interventions**.  

---

## 🎯 Research Questions  
1. **What factors have a significant impact on the severity of traffic accidents?**  
   - What is their relative importance?  
2. **How do different machine learning models compare in predicting the severity of traffic accidents?**  

---

## 📂 Data  
The data utilized in this study originates from the **2023 Road Safety Data** provided by the UK government. It consists of two datasets:  

- **Collision Data**: Provides detailed information on road traffic accidents in the UK that resulted in personal injury.  
- **Vehicle Data**: Includes details of vehicles involved in the recorded accidents.  

---

## 🛠️ Methodology  
The dataset contains numerous independent variables, which may lead to **model overfitting** and **increased computational complexity**. Some irrelevant or less important features may also reduce the accuracy and interpretability of predictions.  

To address this:  
- **Feature selection** is performed using **Random Forest**, which evaluates variable importance and systematically identifies the most relevant predictors.  
- After feature selection, **four different classification algorithms** are applied to predict accident severity. These were chosen for their ability to handle categorical and numerical data, robustness to noise, and adaptability to non-linear patterns.  

### 🔑 Models Used  
- **Random Forest (Breiman, 2001)**: An ensemble of tree-based classifiers. Robust to noise, effective for non-linear patterns, and capable of handling both numerical and categorical data (Titapiccolo et al., 2013).  
- **LightGBM (Ke et al., 2017)**: A gradient boosting framework optimized for speed and scalability. Its histogram-based learning reduces memory usage and training time, ideal for large datasets.  
- **CatBoost (Prokhorenkova et al., 2018)**: A gradient boosting algorithm designed to handle categorical features directly, minimizing information loss during encoding.  
- **XGBoost (Asselman et al., 2023)**: A widely used boosting algorithm with strong regularization, effective in preventing overfitting and handling imbalanced datasets.  

Together, these models provide **diverse approaches** for exploring the dataset comprehensively, ensuring that both linear and non-linear relationships are captured effectively.  

---

## 📊 Expected Contributions  
- A systematic comparison of **machine learning models** for traffic accident severity prediction.  
- Identification of **critical risk factors** influencing accident severity.  
- Insights for **policy-makers and urban planners** to enhance road safety measures.  

---

## 🚀 How to Run (to be updated as project progresses)  
```bash
# Clone the repository
git clone https://github.com/annashen98/traffic-accident-severity.git

# Navigate to project folder
cd traffic-accident-severity

# Run the main script
traffic-accident-severity-analysis.ipynb
