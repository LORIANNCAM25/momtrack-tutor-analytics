# MomTrack Tutor - Data Analytics Capstone

## Overview
MomTrack Tutor is a data-driven educational solution designed for stay-at-home and working moms who want to enhance their child’s learning. This project includes data preparation, SQL querying, Tableau visualization, and business analysis.

## Files Included
- `MomTrack_Tutor_Capstone_Dataset.csv` - Raw dataset used for analysis
- `MomTrack_Tutor_Case_Study.pdf` - Full write-up of business problem, methods, and insights
- Tableau dashboard link: [Insert Your Tableau Public Link Here]

## Technologies Used
- Python (for dataset generation)
- SQL (PostgreSQL syntax)
- Tableau
- Excel (Light cleaning)

## Sample SQL Query
```sql
SELECT Skill_Topic, 
       COUNT(CASE WHEN Milestone_Hit = 'Yes' THEN 1 END)*100.0 / COUNT(*) AS Milestone_Hit_Percentage
FROM momtrack_sessions
GROUP BY Skill_Topic;
