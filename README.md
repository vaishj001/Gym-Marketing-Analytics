# 🏋️‍♂️ Gym Membership Marketing Strategy: Analytics Case Study


📊 A consulting-style marketing analytics project applying segmentation, UX testing, and predictive modeling to improve gym engagement and Premium membership strategy.

---

## 📌 Project Overview

This project simulates a consulting engagement for a mid-sized fitness chain aiming to improve member engagement and grow Premium membership conversions. Using a synthetic gym member dataset, we applied behavioral analytics, persona-driven UX testing, and regression modeling to uncover which member behaviors drive value, and how marketing strategy can be adapted accordingly.

The case reflects a real-world data science approach to marketing optimization in the health and wellness industry.

---

## 🎯 Key Deliverables

- **Exploratory Data Analysis** → Identified trends in satisfaction, visits, and demographic factors to inform modeling and segmentation.
- **Behavior-Based Member Segmentation** → Identified five distinct clusters based on visit frequency, satisfaction, and goal orientation.
- **Persona Development & UX Testing** → Modeled user behavior across digital touchpoints and flagged drop-off points.
- **Predictive Modeling** → Used regression to identify what drives gym usage and assess if Premium upgrade likelihood can be predicted.
- **Strategic Playbook** → Final recommendations focused on engagement, reactivation, offer framing, and campaign personalization.

---

## 🔍 Key Findings

- **Engagement is behavior-led**: Time spent in the gym is highly influenced by visit frequency and satisfaction, not by demographic factors.
- **Demographics are poor predictors**: Age, gender, and proximity to the gym showed no significant relationship with member value or Premium status.
- **Premium upgrades lack a clean pattern**: No single behavioral or demographic factor reliably predicted Premium upgrades, implying decisions are context- or experience-driven.
- **UX issues limit conversion**: Several personas encountered friction in class discovery and the upgrade flow, especially among new members.

---

## 🔬 Data & Methodology

### 📂 Dataset

- 1000-member synthetic dataset with variables such as:
  - Age, gender, distance from gym, fitness goal
  - Monthly visits, time spent per visit, personal training, group classes
  - Membership type, referral status, spend, satisfaction score

### 🧮 Techniques

| Task                        | Tools & Methods                                      |
|-----------------------------|------------------------------------------------------|
| Data Cleaning               | Pandas, NumPy                                        |
| Feature Engineering         | `spend_per_visit`, `visit_satisfaction_interaction` |
| Segmentation                | K-Means Clustering                                   |
| Regression Modeling         | Scikit-learn: Linear & Logistic Regression           |
| UX Analysis                 | Persona-flow evaluation + conversion funnel audit    |
| Visualization               | Seaborn, Matplotlib                                  |

---

## 📊 Analysis Outputs & Results

### Exploratory data analysis

- **Sample size**: 1000 gym members (synthetic dataset)
- **Gender split**: 54.6% male, 45.4% female
- **Age range**: 15–50  
  - Younger males (15–25) favor high-intensity workouts  
  - Older females (40+) show stronger interest in wellness formats
- **Session duration**: No major difference between membership types  
  - Premium: 100.6 minutes/session  
  - Standard: 102.4 minutes/session
- **Top-performing group classes**:  
  - BodyPump (118 participants), XCore (107), Yoga (106)  
  - Clear demand for guided formats; opportunity to scale or repackage lower-performing ones
- **Personal training usage**:  
  - 53.6% of Premium users and 42.3% of Standard users use PT services  
  - Indicates a cross-tier upsell opportunity

### Member segmentation

- **Method**: K-means clustering (k = 5)
- **Segments identified**:
  - **Dedicated Gym Enthusiasts** (23%) – frequent, goal-driven, mid-age range  
  - **Casual Fitness Members** (21%) – infrequent users, wellness-aware  
  - **Personal Training Seekers** (17%) – 1:1 guidance-focused, spend-sensitive  
  - **Group Class Enthusiasts** (19%) – female-skewed, enjoy structured formats  
  - **Wellness & Mindful Members** (20%) – prefer low-impact, holistic offerings

### UX testing & persona evaluation

- **Personas tested**: One per segment (5 total)
- **Features reviewed**: 9 key flows across app and website
- **Highlights**:
  - "Membership Info" and "Instagram Integration" scored highest across personas (+1 to +2)
  - "Supplement Shop" scored -1 from 3 out of 5 personas
  - Class discovery and Premium upgrade flows created friction, especially for new and wellness-focused users

### Regression modeling

- **Linear regression (time spent in gym)**:
  - **R²** = 0.87 (strong model fit)
  - Key predictors:  
    - Monthly visit count (β = +2.00, p < 0.001)  
    - Satisfaction rating (β = +3.64, p < 0.001)  
  - Conclusion: Strong support for behavior-driven engagement

- **Logistic regression (Premium membership prediction)**:
  - **Accuracy**: 97%, but due to label imbalance (~36% Premium)  
  - No statistically significant predictors (all p > 0.05)
  - Odds ratio examples:  
    - Satisfaction rating ≈ 7.87 (p = 0.71)  
    - Annual spend: positive trend, not significant  
  - Conclusion: Cannot reliably predict Premium upgrades; perceived value likely matters more

### Model diagnostics

- **Linear residuals**: Well-distributed; assumptions held
- **Logistic regression**: Multicollinearity caused unstable odds ratios; accuracy inflated due to class imbalance

---

## 💡 Final Recommendations

- Gamify the app for high-frequency users using streaks, progress tracking, and rewards.
- Deploy automated re-engagement campaigns for low-visit members with nudges and free trials.
- Promote social wellness and group classes to increase engagement—particularly among female users.
- Test value-focused Premium bundles (e.g., PT session + class access) across segments.
- Expand and optimize high-performing class types via A/B testing and feedback loops.

---

## 🔮 Future Enhancements

- Capture campaign response and in-app behavior data  
- Survey users for goal-based personalization  
- Model churn likelihood and time-to-upgrade curves  
- Build real-time triggers for marketing automation

---

## 📂 Project Structure

```
├── gym_data/                          # Processed dataset
├── marketing_notebook.ipynb/          # Jupyter Notebook for analysis
├── personas_uxtesting.pdf/            # Marketing & User Personas and UX Testing
├── final_presentation.pdf/            # Final slide deck covering the entire project
├── professional_memo.pdf/             # Professional memo to executives
├── README.md                          # Project Overview (this file)
```
