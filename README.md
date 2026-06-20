# Investigating the Impact of Social Media Usage on University Admission Success Among Gen-Z Students

By: Caithlyn Natalie 郭虹秀
DSCP Final Project

## 1. Introduction & Background
This research project investigates the correlation between daily social media usage and university admission success by analyzing how digital habits influence the students academic performance and extracurricular engagement. By utilizing a dataset of 1,000,000 students, the study aims to validate an academic trade-off hypothesis, where higher social_media_hours may lead to a decrease in high_school_gpa and volunteer_hours. The research also explores the impact of digital consumption on subjective admission criteria like the essay_score, identifying whether excessive social media time begins to noticeably decrease a candidate's probability of admission_status. 
Dataset : https://www.kaggle.com/datasets/sharmajicoder/genn-z-college-admission-dataset/data

## 2. Research Objectives
* **To test the Academic Trade-off Hypothesis** by measuring the impact of daily social media hours on quantitative metrics (High School GPA and accumulated volunteer hours).
* **To assess digital consumption's influence on qualitative admission criteria**, determining whether high screen time correlates with a noticeable decline in standardized essay scores.
* **To identify the ultimate threshold** where daily social media habits begin to significantly alter a candidate's overall probability of university admission.

### Data Preprocessing & Cleaning Pipeline
The analytical pipeline was built using Python's libraries: **Pandas (`pd`)** 

1. **Feature Isolation:** The dataset was filtered to retain 5 core academic and behavioral attributes: `social_media_hours`, `high_school_gpa`, `volunteer_hours`, `essay_score`, and `admission_status`
2. **Data Cleaning:** Missing or incomplete records were handled via row-wise omission (`.dropna()`) to secure statistical integrity
3. **Data Transformation:** All variables were strictly cast into numerical formats using `pd.to_numeric()` to prevent data type mismatches during matrix calculations
   * **Low Usage:** 0 – 3 hours/day
   * **Medium Usage:** 3 – 6 hours/day
   * **High Usage:** 6+ hours/day

### Statistical Correlations
The calculated mathematical correlation between daily social media hours and all critical academic metrics yielded an absolute value of **0.00**, indicating absolute zero linear relationship:
* **Social Media vs. GPA:** -0.00
* **Social Media vs. Volunteer Hours:** 0.00
* **Social Media vs. Essay Score:** -0.00
* **Social Media vs. Admission Status:** 0.00

### Demographic & Outcome Distributions
* **Sample Distribution:** The majority of students fall into the **Medium Users** category at **59.58%**, followed by **Low Users (21.02%)** and **High Users (19.40%)**.
* **Admission Output Summary:** The output reveals an identical, uniform proportional ratio of admitted versus rejected students across all three tiers.
  * **Low Usage (0-3h):** 70,117 Admitted vs. 9,414 Not Admitted
  * **Medium Usage (3-6h):** 198,803 Admitted vs. 26,687 Not Admitted
  * **High Usage (6h+):** 64,785 Admitted vs. 8,630 Not Admitted
 
### Visual Analysis
#### Chart 1: Demographic Segmentation (Pie Chart)
#### Chart 2: Social Media Hours vs. Admission Probability (Line Chart)
#### Chart 3: Social Media Hours vs. High School GPA (Line Chart)
#### Chart 4: Social Media Hours vs. Volunteer Time (Line Chart)
#### Chart 5: Social Media Hours vs. Essay Score (Line Chart)

## 6. Conclusion
Based on the analysis over the dataset of 1,000,000 students, the Academic Trade-off Hypothesis is rejected. The evidence demonstrates that daily social media usage behaves as a completely neutral variable within this population, as proven by correlation coefficient of exactly 0.00 across all academic performance and admission vectors. When segmented into low, medium, and high digital usage, the conditional means for all performance metrics remained completely stagnant, showing an average GPA locked at ~3.19, extracurricular community service stable at ~99.4 hours, and standardized essay scores at ~74.9 out of 100. This absolute lack of statistical variance indicates that heavy digital screen time does not displace structured academic activities or degrade a student's cognitive and qualitative writing capabilities. Lastly, the probability of university admission is a horizontal of a success rate of ~88%, showing an identical proportional ratio of admitted versus rejected students regardless of screen time.
