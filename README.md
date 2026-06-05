# Employee-Burnout-Risk-Prediction-System

## 📌 Project Overview
Employee burnout is a leading cause of reduced productivity, increased attrition, and poor employee well-being. This project simulates a real-world HR Analytics use case. The objective is to develop a predictive analytics solution capable of estimating an employee's **Burnout Risk Score** (on a scale of 0–100) using workplace, productivity, and lifestyle-related factors.

This project was developed as part of a **Machine Learning Internship Assignment** to demonstrate end-to-end data processing, exploratory data analysis (EDA), predictive modeling, and the extraction of actionable business insights.

## 📊 Dataset Information
The dataset consists of 1,000 employee records with the following features:
- **Workplace Metrics:** `years_experience`, `weekly_work_hours`, `meetings_per_week`, `emails_sent_per_day`, `projects_handled`, `remote_days_per_month`
- **Lifestyle & Well-being:** `age`, `sleep_hours`, `stress_level`, `exercise_hours_week`, `sick_leaves_year`
- **Performance:** `productivity_score`
- **Target Variable:** `burnout_risk_score` (0-100 scale)

## ⚙️ Methodology & Phases

### Phase 1: Exploratory Data Analysis (EDA)
- Conducted missing value analysis (Dataset was clean; 0 missing values).
- Visualized feature distributions using histograms and box plots for outlier detection.
- Generated a **Correlation Heatmap** revealing that `stress_level` and `weekly_work_hours` are the highest positive drivers of burnout, while `sleep_hours` and `exercise_hours_week` act as negative drivers (mitigators).

### Phase 2: Data Preprocessing
- Dropped irrelevant identifiers (`employee_id`).
- Split the data into **80% Training** and **20% Testing** sets.
- Applied **Feature Scaling (`StandardScaler`)** to ensure all features contributed equally to the model and to allow for accurate coefficient interpretation.

### Phase 3 & 4: Model Development & Evaluation
Developed a **Linear Regression** model using `Scikit-Learn`. Evaluated using standard regression metrics:
- **Mean Absolute Error (MAE)**
- **Mean Squared Error (MSE)**
- **Root Mean Squared Error (RMSE)**
- **R² Score** *(Indicates strong explanatory power of the model)*

### Phase 5: Business Insights & Bonus Analysis
Using the trained model, simulated three "What-If" business scenarios to provide quantitative backing for HR recommendations:
1. **Scenario 1:** Reduced weekly working hours by 10%.
2. **Scenario 2:** Assumed employees increase their sleep by 1 hour per day.
3. **Scenario 3:** Assumed employees exercise 3 additional hours per week.

## 💡 Key Business Recommendations
1. **Cap Maximum Work Hours:** Limit weekly working hours, as the model showed a severe spike in burnout risk beyond the 50-hour mark.
2. **Implement Wellness Initiatives:** Incentivize sleep hygiene and fitness. Our simulations proved that +1 hour of sleep and +3 hours of weekly exercise drastically reduce average company burnout scores.
3. **Proactive HR Monitoring:** Utilize the model's coefficients to build a dashboard that flags employees with stress levels ≥ 8 and high meeting/email loads for early intervention.

## 🛠️ Installation & Usage

1. **Clone the repository:**
   ```bash
   git clone https://github.com/ullhasykumar/Employee-Burnout-Risk-Prediction-System.git
   cd Employee-Burnout-Risk-Prediction-System
2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt

3. **Run the Jupyter Notebook or the Python file:**
   
   Jupyter Notebook : Open `notebooks/Employee-Burnout-Risk-Prediction-System.ipynb` and run the cells.
   
   Python file : Open `src/Employee-Burnout-Risk-Prediction-System.py` and run the program.

----------------------------------------------------------------------------------------------------------------------------------------------------------------

**## Let's Connect!!**

**Thank you for taking the time to check out my repository. This marks my first foray into the world of Machine Learning!**

**I am highly receptive to constructive feedback. If you spot any areas for improvement or just want to chat about data science, please feel free to correct me** **or drop a message. I'd love to connect with like-minded individuals!**

📫 **To contact me: checkout my github userpage** 

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
   
