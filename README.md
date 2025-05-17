#  MomTrack Tutor – Capstone Project

**MomTrack Tutor** is a data-driven educational solution designed for stay at home and working moms who want to enhance their child’s early development through personalized, skill based tutoring. This project includes data preparation, SQL querying, Tableau visualization, and business insights.

---

##  Files Included

* `MomTrack_Tutor_Capstone_Dataset.csv` — Raw dataset used for analysis
* `MomTrack_Tutor_Case_Study.pdf` — Full write up of business task, methods, analysis, and conclusions
* [🔗 Tableau Dashboard](INSERT-YOUR-LINK-HERE) — Visual representation of analysis (hosted on Tableau Public)

---

## 🛠 Technologies Used

* **Python** — for synthetic dataset generation
* **SQL (PostgreSQL)** — for querying and insight extraction
* **Tableau** — for data visualization and storytelling
* **Excel** — for light data cleaning and quick EDA

---

## 📈 Sample SQL Query

```sql
SELECT 
    Skill_Topic, 
    COUNT(CASE WHEN Milestone_Hit = 'Yes' THEN 1 END) * 100.0 / COUNT(*) AS Milestone_Hit_Percentage
FROM 
    momtrack_sessions
GROUP BY 
    Skill_Topic;
```

