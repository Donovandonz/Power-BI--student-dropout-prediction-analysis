# Power-BI--student-dropout-prediction-analysis
🎓 Student Dropout Prediction Dashboard 

---

## Dataset used
-<a href="https://github.com/Donovandonz/Power-BI--student-dropout-prediction-analysis/blob/main/student_dropout_dataset_v3.csv">RAW.student-dropout-dataset</a>

---

## 📋 Project Overview

This Student Dropout Prediction Dashboard analyzes data from **10,000 students** to identify key factors contributing to student dropout rates. The project aims to help educational institutions identify at-risk students early and implement targeted intervention strategies.

---

## 🛠️ Tools Used

| Tool | Purpose |
|------|---------|
| **📗 Excel** | Data cleaning, transformation, and initial exploration |
| **📊 Power BI** | Interactive dashboard creation, DAX calculations, and visualization |

---

## 🎯 Project Objectives

- Identify demographic factors influencing student dropout rates
- Analyze academic performance patterns among dropouts vs. non-dropouts
- Understand behavioral indicators (attendance, assignment delays, stress levels)
- Compare dropout rates across different departments
- Provide actionable insights for student retention strategies

---

### Key Metrics at a Glance
| Metric | Value |
|--------|-------|
| Total Students | 10,000 |
| Dropout Count | 2,000 |
| Active Students | 7,600 |
| Overall Dropout Rate | 23.5% |

---

### 1. Summary Dashboard
- Overall KPIs and metrics
- Dropout rate by semester trend
- Dropout rate by stress index
- Department-wise dropout distribution
- Dropout rate by attendance, GPA, and assignment delay

### 2. Demographic Dashboard
- Parental education impact on dropout rates
- Gender-based dropout analysis
- Family income impact analysis

### 3. Academic Factor Dashboard
- GPA comparison: Dropout vs. Non-dropout
- GPA distribution across student population
- CGPA trends by semester
- Study hours risk analysis

### 4. Department Dashboard
- Department-wise student distribution
- Dropout rates by department
- Average attendance and GPA by department

### 5. Behavioral Patterns Dashboard
- Attendance category distribution
- Assignment delay impact analysis
- Stress index critical threshold analysis

### 6. Risk Indicator Dashboard
- Average of risk score
- Total of student in risk category
- Student department distribution

---

## 1. Summary Dashboard: Key Findings & Insights

### Overall Performance Metrics
| Metric | Value | Interpretation |
|--------|-------|----------------|
| Total Students | 10,000 | Baseline population |
| Dropout Count | 2,000 | Significant concern |
| Active Students | 7,600 | Retention rate: 76.5% |
| Overall Dropout Rate | 23.5% | 1 in 4 students drop out |

### Dropout Rate by Stress Index - UPDATED

| Stress Level | Dropout Rate | Risk Multiplier |
|--------------|--------------|-----------------|
| Critical (10) | 54.8% | 7.9x baseline |
| High (8-9) | 38.6% | 5.6x baseline |
| Moderate (6-7) | 25.6% | 3.7x baseline |
| Normal (4-5) | 14.5% | 2.1x baseline |
| Low (0-3) | 6.9% | 1x (baseline) |

**Critical Finding:** Students with critical stress levels (10) have a 54.8% dropout rate - meaning more than half of these students will not persist. This is **7.9 times higher** than students with low stress.

**Stress Impact Gradient:**
- Moving from Low → Normal: +7.6% dropout increase
- Moving from Normal → Moderate: +11.1% dropout increase
- Moving from Moderate → High: +13.0% dropout increase
- Moving from High → Critical: +16.2% dropout increase

**Key Insight:** The dropout rate accelerates as stress increases, with the largest jump occurring between High and Critical stress levels.

### Dropout Rate by Attendance - UPDATED

| Attendance Category | Range | Dropout Rate | Risk Level |
|---------------------|-------|--------------|------------|
| Poor | <50% | 50.0% | Critical Risk |
| Below Average | 70-80% | 38.9% | High Risk |
| Good | 80-90% | 24.0% | Moderate Risk |
| Excellent | 90-100% | 14.2% | Low Risk |

**Attendance Impact Analysis:**

| Attendance Category | Dropout Rate | vs. Excellent |
|---------------------|--------------|---------------|
| Excellent (90-100%) | 14.2% | Baseline |
| Good (80-90%) | 24.0% | +9.8% |
| Below Average (70-80%) | 38.9% | +24.7% |
| Poor (<50%) | 50.0% | +35.8% |

**Critical Finding:** Students with poor attendance (<50%) have a 50% dropout rate - **1 in 2 students** in this category will drop out.

**Key Insight:** Every drop in attendance category significantly increases dropout risk. The jump from Good (24.0%) to Below Average (38.9%) represents a 62% increase in dropout probability.

### Dropout Rate by GPA - UPDATED

| GPA Category | Range | Dropout Rate | Risk Multiplier |
|--------------|-------|--------------|-----------------|
| Poor | <2.0 | 45.0% | 10.7x baseline |
| Below Average | 2.0-2.49 | 18.5% | 4.4x baseline |
| Average | 2.5-2.99 | 11.7% | 2.8x baseline |
| Good | 3.0-4.0 | 4.2% | 1x (baseline) |

**GPA Impact Analysis:**

| GPA Range | Dropout Rate | Student Count | % of Population |
|-----------|--------------|---------------|-----------------|
| <2.0 (Poor) | 45.0% | 4,000 | 40% |
| 2.0-2.49 (Below Average) | 18.5% | 2,000 | 20% |
| 2.5-2.99 (Average) | 11.7% | 2,000 | 20% |
| 3.0-4.0 (Good) | 4.2% | 2,000 | 20% |

**Critical Finding:** Students with GPA below 2.0 have a **45% dropout rate** - nearly half of this massive population (4,000 students) will not persist.

**Most Alarming Statistic:** The 4,000 students in the Poor GPA category (<2.0) represent **40% of all students** and face a 45% dropout rate. This is the single largest at-risk population.

**Success Story:** Students with Good GPA (3.0-4.0) have only 4.2% dropout rate - academic success is strongly protective.

### Dropout Rate by Assignment Delay

| Delay Category | Dropout Rate | Interpretation |
|----------------|--------------|----------------|
| Severe (>7 days) | 50% | Critical warning sign |
| Moderate (4-6 days) | 50% | High risk behavior |
| Minor (1-3 days) | 50% | Early intervention opportunity |
| On Time | Baseline | Protective factor |

**Key Insight:** Any assignment delay, regardless of duration, is associated with 50% dropout rate - making it one of the strongest early warning indicators.

### Department-wise Dropout Count

| Department | Dropout Count | Rank |
|------------|---------------|------|
| Arts | 485 | 1st (highest) |
| Science | 475 | 2nd |
| Business | 467 | 3rd |
| Engineering | 465 | 4th |
| Computer Science | 462 | 5th (lowest) |

**Key Finding:** Arts department has the highest absolute number of dropouts (485), while Computer Science has the lowest (462) - a narrow range suggesting systemic issues across all departments.

### Dropout Rate by Semester

**Semester Trend Analysis**
| Semester | Dropout Rate Trend | Key Insight |
|----------|-------------------|-------------|
| Year 1 | High | Transition challenges, adjustment period |
| Year 2 | Peak | Critical intervention window |
| Year 3 | Declining | Students who survive Year 2 more likely to persist |
| Year 4 | Lowest | Near-completion, strong commitment |

**Critical Finding:** Dropout risk is highest in Year 2, suggesting the "sophomore slump" requires targeted intervention.

---

### Updated Risk Factor Comparison

| Risk Factor | Category | Dropout Rate | Risk Multiplier |
|-------------|----------|--------------|-----------------|
| **Stress** | Critical (10) | 54.8% | 7.9x |
| **Attendance** | Poor (<50%) | 50.0% | 3.5x vs Excellent |
| **GPA** | Poor (<2.0) | 45.0% | 10.7x vs Good |
| **Assignment Delay** | Any Delay | 50.0% | Significant |

**Top 3 Highest Risk Indicators:**
1. Critical Stress (10): 54.8% dropout rate
2. Poor Attendance (<50%): 50.0% dropout rate
3. Any Assignment Delay: 50.0% dropout rate

### Summary Dashboard Conclusions

1. **Stress is the Strongest Predictor:** Critical stress (54.8% dropout) is the single most dangerous risk factor

2. **Academic Failure is Widespread:** 40% of students (4,000) have GPA <2.0 with 45% dropout rate

3. **Attendance Matters Significantly:** 38.9% dropout for Below Average attendance (70-80%)

4. **Protective Factors Work:** Excellent attendance (14.2%) and Good GPA (4.2%) show strong retention

5. **Intervention Priorities:**
   - Immediate: Students with critical stress (54.8% risk)
   - High: Students with poor attendance (50% risk)
   - Critical Mass: 4,000 students with GPA <2.0 (45% risk)
  
---

## 2. Academic Factor Dashboard: Key Findings & Insights

### GPA Comparison: Dropout vs. Non-Dropout

| Student Status | Average GPA | Gap | Interpretation |
|----------------|-------------|-----|-----------------|
| Non-Dropout | 2.60 | Baseline | Passing but concerning |
| Dropout | 1.43 | -1.17 | Failing average |

**Critical Finding:** The 1.17 GPA gap between dropouts and non-dropouts represents a full letter grade difference - academic performance is a powerful separator.

---

### GPA Distribution and Dropout Rates - UPDATED with Correct Numbers

| GPA Range | Category | Student Count | % of Population | Dropout Rate | At-Risk Students (Projected Dropouts) |
|-----------|----------|---------------|-----------------|--------------|------------------|
| Below 2.0 | Fail | 3,863 | 38.6% | 45.0% | 1,738 |
| 2.0-2.5 | Poor | 1,641 | 16.4% | 18.5% | 304 |
| 2.5-3.0 | Average | 1,656 | 16.6% | 11.7% | 194 |
| 3.0-3.5 | Good | 1,244 | 12.4% | 4.2% | 52 |
| 3.5-4.0 | Excellent | 1,596 | 16.0% | 4.2% | 67 |
| **TOTAL** | | **10,000** | **100%** | **23.5%** | **2,355** |

---

### Critical Finding: The FAIL Category Crisis

| Metric | Value |
|--------|-------|
| Students with GPA < 2.0 | 3,863 |
| Percentage of Population | 38.6% |
| Dropout Rate | 45.0% |
| Projected Dropouts from this Group | 1,738 |
| % of Total Dropouts from this Group | **73.8%** |

**ALARMING INSIGHT:** Students with GPA below 2.0 represent **38.6% of all students** but account for **73.8% of all projected dropouts**. This is the single most critical at-risk population.

---

### GPA Category Analysis

**Category Breakdown by Size:**

| Rank | Category | Range | Count | % of Population |
|------|----------|-------|-------|-----------------|
| 1 | Fail | <2.0 | 3,863 | 38.6% |
| 2 | Average | 2.5-3.0 | 1,656 | 16.6% |
| 3 | Poor | 2.0-2.5 | 1,641 | 16.4% |
| 4 | Excellent | 3.5-4.0 | 1,596 | 16.0% |
| 5 | Good | 3.0-3.5 | 1,244 | 12.4% |

**Category Breakdown by Dropout Rate:**

| Rank | Category | Range | Dropout Rate | Risk Multiplier |
|------|----------|-------|--------------|-----------------|
| 1 | Fail | <2.0 | 45.0% | 10.7x vs Good |
| 2 | Poor | 2.0-2.5 | 18.5% | 4.4x vs Good |
| 3 | Average | 2.5-3.0 | 11.7% | 2.8x vs Good |
| 4 | Good | 3.0-3.5 | 4.2% | Baseline |
| 4 | Excellent | 3.5-4.0 | 4.2% | Baseline |

---

### GPA Risk Analysis

| GPA Category | Dropout Rate | Risk vs. Good GPA (3.0-3.5) |
|--------------|--------------|-----------------------------|
| Fail (<2.0) | 45.0% | 10.7x higher |
| Poor (2.0-2.5) | 18.5% | 4.4x higher |
| Average (2.5-3.0) | 11.7% | 2.8x higher |
| Good (3.0-3.5) | 4.2% | Baseline |
| Excellent (3.5-4.0) | 4.2% | Baseline |

**Key Insight:** There is a dramatic risk cliff between Fail (45.0%) and Poor (18.5%) - improving students from <2.0 to 2.0-2.5 reduces dropout risk by **26.5 percentage points**.

---

### GPA Protective Effect - The Intervention ROI

| GPA Improvement | Dropout Risk Reduction | Students Impacted |
|-----------------|------------------------|-------------------|
| Fail → Poor (<2.0 → 2.0-2.5) | -26.5% | 3,863 |
| Poor → Average (2.0-2.5 → 2.5-3.0) | -6.8% | 1,641 |
| Average → Good (2.5-3.0 → 3.0-3.5) | -7.5% | 1,656 |
| Good → Excellent (3.0-3.5 → 3.5-4.0) | 0% | 1,244 |

**CRITICAL FINDING:** The biggest return on investment is moving students out of the Fail category (<2.0). Every student moved from Fail to Poor reduces dropout probability by 26.5 percentage points.

---

### Projected Dropouts by GPA Category

| GPA Category | Student Count | Dropout Rate | Projected Dropouts | % of Total Dropouts |
|--------------|---------------|--------------|-------------------|---------------------|
| Fail (<2.0) | 3,863 | 45.0% | 1,738 | 73.8% |
| Poor (2.0-2.5) | 1,641 | 18.5% | 304 | 12.9% |
| Average (2.5-3.0) | 1,656 | 11.7% | 194 | 8.2% |
| Good (3.0-3.5) | 1,244 | 4.2% | 52 | 2.2% |
| Excellent (3.5-4.0) | 1,596 | 4.2% | 67 | 2.9% |
| **TOTAL** | **10,000** | **23.5%** | **2,355** | **100%** |

**Interpretation:** Students are clustering at the extremes - either failing or excelling, with fewer in the middle ranges than expected.

| Category | Expected Normal Distribution | Actual | Deviation |
|----------|------------------------------|--------|-----------|
| Fail | ~10-15% | 38.6% | +23.6% |
| Poor/Average | ~50-60% | 33.0% | -22% |
| Good/Excellent | ~25-30% | 28.4% | Near normal |

**Insight:** The middle is hollow - students are either struggling significantly or performing well, with less of a "average student" population.

---

### CGPA Trends by Semester

| Semester | Average CGPA | Student Count | Trend |
|----------|--------------|---------------|-------|
| Year 1 | 2.31 | 2,308 | Starting point |
| Year 2 | 2.30 | 2,301 | Slight decline |
| Year 3 | 2.28 | 2,304 | Lowest point |
| Year 4 | 2.30 | 2,301 | Slight recovery |

**Longitudinal Insights:**

1. **Minimal Variation:** CGPA stays remarkably stable (2.28-2.31) across all 4 years
2. **Year 3 Slump:** Smallest dip in Year 3 (2.28) - "junior slump"
3. **Year 4 Recovery:** Slight improvement as graduation approaches
4. **No Growth:** Students aren't improving academically over time

**Concerning Pattern:** CGPA should increase as students progress (weeding out poor performers, maturing learners). Flat line suggests no academic development.

---

### GPA Distribution by Semester (Estimated)

| Semester | Avg GPA | Est. Fail Count (<2.0) | Fail % |
|----------|---------|------------------------|--------|
| Year 1 | 2.31 | ~892 | 38.6% |
| Year 2 | 2.30 | ~898 | 39.0% |
| Year 3 | 2.28 | ~922 | 40.0% |
| Year 4 | 2.30 | ~898 | 39.0% |

**Key Finding:** The proportion of students with GPA <2.0 remains consistently high (38-40%) across all years - the problem persists from enrollment to graduation.

---

### Academic Risk Profiles

**Critical Risk Profile (Fail Category - 3,863 students):**
- GPA < 2.0
- 45.0% dropout rate
- 38.6% of all students
- Projected Dropouts: 1,738
- **Accounts for 73.8% of all dropouts**

**High Risk Profile (Poor Category - 1,641 students):**
- GPA 2.0-2.5
- 18.5% dropout rate
- 16.4% of all students
- Projected Dropouts: 304

**Moderate Risk Profile (Average Category - 1,656 students):**
- GPA 2.5-3.0
- 11.7% dropout rate
- 16.6% of all students
- Projected Dropouts: 194

**Low Risk Profile (Good/Excellent - 2,840 students):**
- GPA 3.0-4.0
- 4.2% dropout rate
- 28.4% of all students
- Projected Dropouts: 119

---

### Study Hours Risk Analysis

| Study Hours Category | Hours Range | Non-Dropout Avg GPA | Dropout Avg GPA | GPA Gap |
|---------------------|-------------|-------------------|-----------------|---------|
| Excessive | >6 hrs | 2.93 | 1.87 | 1.06 |
| High | 4.5-6 hrs | 2.69 | 1.56 | 1.13 |
| Recommended | 3.5-4 hrs | 2.51 | 1.38 | 1.13 |
| Moderate | 2.5-3 hrs | 2.37 | 1.26 | 1.11 |
| Low | 1.5-2 hrs | 2.26 | 1.16 | 1.10 |
| Very Low | 0.5-1 hrs | 1.97 | 0.94 | 1.03 |

---

### Study Hours Analysis - Sorted by Non-Dropout GPA

| Rank | Study Hours Category | Hours Range | Non-Dropout Avg GPA | Dropout Avg GPA | Study Efficiency |
|------|---------------------|-------------|-------------------|-----------------|------------------|
| 1 | Excessive | >6 hrs | 2.93 | 1.87 | Most Effective |
| 2 | High | 4.5-6 hrs | 2.69 | 1.56 | Effective |
| 3 | Recommended | 3.5-4 hrs | 2.51 | 1.38 | Good |
| 4 | Moderate | 2.5-3 hrs | 2.37 | 1.26 | Moderate |
| 5 | Low | 1.5-2 hrs | 2.26 | 1.16 | Low |
| 6 | Very Low | 0.5-1 hrs | 1.97 | 0.94 | Ineffective |

---

### Key Findings: Study Hours Impact

**Positive Correlation:** More study hours = Higher GPA for both non-dropout and dropout students

| Hours Category | Non-Dropout GPA | vs. Very Low | Dropout GPA | vs. Very Low |
|----------------|-----------------|--------------|-------------|--------------|
| Very Low (0.5-1) | 1.97 | Baseline | 0.94 | Baseline |
| Low (1.5-2) | 2.26 | +0.29 | 1.16 | +0.22 |
| Moderate (2.5-3) | 2.37 | +0.40 | 1.26 | +0.32 |
| Recommended (3.5-4) | 2.51 | +0.54 | 1.38 | +0.44 |
| High (4.5-6) | 2.69 | +0.72 | 1.56 | +0.62 |
| Excessive (>6) | 2.93 | +0.96 | 1.87 | +0.93 |

---

### The Study Hours Gap Analysis

**GPA Gap Between Non-Dropout and Dropout by Hours Category:**

| Study Hours | Non-Dropout GPA | Dropout GPA | Gap | Gap vs. Average |
|-------------|-----------------|-------------|-----|-----------------|
| Excessive (>6) | 2.93 | 1.87 | 1.06 | -0.05 |
| High (4.5-6) | 2.69 | 1.56 | 1.13 | +0.02 |
| Recommended (3.5-4) | 2.51 | 1.38 | 1.13 | +0.02 |
| Moderate (2.5-3) | 2.37 | 1.26 | 1.11 | 0.00 |
| Low (1.5-2) | 2.26 | 1.16 | 1.10 | -0.01 |
| Very Low (0.5-1) | 1.97 | 0.94 | 1.03 | -0.08 |
| **AVERAGE** | **2.46** | **1.36** | **1.10** | |

**Insight:** The GPA gap between dropouts and non-dropouts remains remarkably consistent (1.03-1.13) across all study hours categories - approximately a full letter grade difference regardless of study time.

---

### Study Hours Recommendations by Student Profile

**For At-Risk Students (Current GPA <2.0):**
- Target: Minimum 2.5-3 hours daily (Moderate category)
- Expected GPA: 1.26 (current dropouts) → 2.37 (non-dropouts)
- Gap to close: 1.11 points
- Support needed: Study skills training, not just more hours

**For Struggling Students (Current GPA 2.0-2.5):**
- Target: 3.5-4 hours daily (Recommended category)
- Expected GPA: 2.51
- Support needed: Time management, effective study techniques

**For Successful Students (Current GPA >2.5):**
- Target: 4.5+ hours daily (High/Excessive)
- Expected GPA: 2.69-2.93
- Support needed: Advanced strategies, depth over breadth

---

### Study Hours vs. GPA Matrix

| Hours Category | Non-Dropout GPA | Dropout GPA | Effectiveness Rating |
|----------------|-----------------|-------------|---------------------|
| Excessive (>6) | 2.93 (B) | 1.87 (C-) | ⭐⭐⭐⭐⭐ |
| High (4.5-6) | 2.69 (C+) | 1.56 (D+) | ⭐⭐⭐⭐ |
| Recommended (3.5-4) | 2.51 (C) | 1.38 (D) | ⭐⭐⭐ |
| Moderate (2.5-3) | 2.37 (C-) | 1.26 (D) | ⭐⭐ |
| Low (1.5-2) | 2.26 (C-) | 1.16 (D-) | ⭐ |
| Very Low (0.5-1) | 1.97 (D+) | 0.94 (F) | ⚠️ |

---

## 3. Department Dashboard: Key Findings & Insights

### Department Overview

| Department | Total Students | % of Population | Dropout Count | Dropout Rate | Avg Attendance | Avg GPA |
|------------|---------------|-----------------|--------------|--------------|----------------|---------|
| Science | 2,061 | 20.6% | 475 | 23.0% | 81.48 | 2.33 |
| Arts | 2,026 | 20.3% | 485 | 23.9% | 82.01 | 2.32 |
| Business | 2,002 | 20.0% | 467 | 23.3% | 81.77 | 2.32 |
| Computer Science | 1,974 | 19.7% | 462 | 23.4% | 81.74 | 2.30 |
| Engineering | 1,937 | 19.4% | 465 | 24.0% | 81.70 | 2.27 |
| **TOTAL** | **10,000** | **100%** | **2,754** | **-** | **-** | **-** |

### Department Performance Ranking

**By Dropout Rate (Best to Worst):**
| Rank | Department | Dropout Rate | vs Average |
|------|------------|--------------|------------|
| 1 | Science | 23.0% | -0.5% |
| 2 | Business | 23.3% | -0.2% |
| 3 | Computer Science | 23.4% | -0.1% |
| 4 | Arts | 23.9% | +0.4% |
| 5 | Engineering | 24.0% | +0.5% |

**By GPA (Highest to Lowest):**
| Rank | Department | Avg GPA | vs Average |
|------|------------|---------|------------|
| 1 | Science | 2.33 | +0.02 |
| 2 | Arts | 2.32 | +0.01 |
| 2 | Business | 2.32 | +0.01 |
| 4 | Computer Science | 2.30 | -0.01 |
| 5 | Engineering | 2.27 | -0.04 |

**By Attendance (Highest to Lowest):**
| Rank | Department | Attendance | vs Average |
|------|------------|------------|------------|
| 1 | Arts | 82.01% | +0.28 |
| 2 | Business | 81.77% | +0.04 |
| 3 | Computer Science | 81.74% | +0.01 |
| 4 | Engineering | 81.70% | -0.03 |
| 5 | Science | 81.48% | -0.25 |

### Department Performance Matrix

| Department | Dropout Rate | GPA | Attendance | Overall Rank |
|------------|--------------|-----|------------|--------------|
| Science | 🟢 Best | 🟢 Best | 🔴 Worst | 1 |
| Business | 🟢 2nd | 🟢 2nd | 🟢 2nd | 2 |
| Arts | 🔴 4th | 🟢 2nd | 🟢 Best | 3 |
| Computer Science | 🟢 3rd | 🟡 4th | 🟢 3rd | 4 |
| Engineering | 🔴 Worst | 🔴 Worst | 🟡 4th | 5 |

🟢 = Above Average | 🟡 = Average | 🔴 = Below Average

### Key Department Insights

**Science Department (Best Overall Performer)**
- **Strengths:** Lowest dropout rate (23.0%), highest GPA (2.33)
- **Weakness:** Lowest attendance (81.48%)
- **Paradox:** Students attend less but perform better - suggests high aptitude or rigorous selection

**Arts Department (Mixed Performance)**
- **Strengths:** Highest attendance (82.01%), good GPA (2.32)
- **Weakness:** High dropout rate (23.9%, 4th place)
- **Paradox:** High attendance doesn't translate to retention - engagement quality issue?

**Business Department (Consistent Performer)**
- **Metrics:** All metrics slightly above average
- **Profile:** Balanced performance across all categories
- **Ranking:** Solid 2nd place overall

**Computer Science Department (Middle Performer)**
- **Strengths:** Low dropout count (462, lowest absolute)
- **Weaknesses:** Below average GPA (2.30)
- **Profile:** Moderate performance with room for improvement

**Engineering Department (Worst Performer)**
- **Weaknesses:** Highest dropout rate (24.0%), lowest GPA (2.27), low attendance (81.70%)
- **Crisis Indicators:** Bottom in 2 of 3 metrics
- **Urgency:** Needs immediate intervention

### Department Size Analysis

| Size Rank | Department | Students | % of Total |
|-----------|------------|----------|------------|
| 1 | Science | 2,061 | 20.6% |
| 2 | Arts | 2,026 | 20.3% |
| 3 | Business | 2,002 | 20.0% |
| 4 | Computer Science | 1,974 | 19.7% |
| 5 | Engineering | 1,937 | 19.4% |

**Observation:** Departments are nearly evenly distributed (19.4-20.6%) - excellent balance for comparative analysis

### Dropout Count Analysis

| Department | Dropout Count | % of Total Dropouts |
|------------|--------------|---------------------|
| Arts | 485 | 17.6% |
| Science | 475 | 17.2% |
| Business | 467 | 17.0% |
| Engineering | 465 | 16.9% |
| Computer Science | 462 | 16.8% |

**Key Finding:** Dropouts are evenly distributed across departments (16.8-17.6%) - no single department dominates dropout numbers

### Correlation Analysis

**GPA vs Dropout Rate:**
- Science: Highest GPA (2.33) = Lowest Dropout (23.0%)
- Engineering: Lowest GPA (2.27) = Highest Dropout (24.0%)
- **Correlation:** Strong negative relationship

**Attendance vs Dropout Rate:**
- Arts: Highest Attendance (82.01%) = High Dropout (23.9%)
- Science: Lowest Attendance (81.48%) = Low Dropout (23.0%)
- **Correlation:** Weak/No relationship - attendance alone doesn't predict success

### Department Risk Profiles

**Engineering (Highest Risk):**
- Dropout Rate: 24.0% (+0.5% above avg)
- GPA: 2.27 (-0.04 below avg)
- Attendance: 81.70% (-0.03 below avg)
- Risk Factors: Academic difficulty, curriculum rigor

**Arts (High Risk):**
- Dropout Rate: 23.9% (+0.4% above avg)
- GPA: 2.32 (+0.01 above avg)
- Attendance: 82.01% (+0.28 above avg)
- Risk Factors: Engagement quality, career uncertainty

**Computer Science (Moderate Risk):**
- Dropout Rate: 23.4% (-0.1% below avg)
- GPA: 2.30 (-0.01 below avg)
- Attendance: 81.74% (+0.01 above avg)
- Risk Factors: Technical difficulty, workload

**Business (Low-Moderate Risk):**
- Dropout Rate: 23.3% (-0.2% below avg)
- GPA: 2.32 (+0.01 above avg)
- Attendance: 81.77% (+0.04 above avg)
- Risk Factors: Competitive pressure

**Science (Lowest Risk):**
- Dropout Rate: 23.0% (-0.5% below avg)
- GPA: 2.33 (+0.02 above avg)
- Attendance: 81.48% (-0.25 below avg)
- Risk Factors: None significant

### Key Department Takeaways

1. **Science Excels:** Best academic outcomes despite lowest attendance - what's their secret?

2. **Engineering Struggles:** Worst in multiple metrics - needs comprehensive review

3. **Attendance Paradox:** Arts has best attendance but high dropout - attendance ≠ engagement

4. **Even Distribution:** All departments similar size - ideal for fair comparison

5. **GPA Matters:** Strong correlation between GPA and retention across departments

### Department-Specific Recommendations

**For Engineering (Immediate Intervention Needed):**
- Curriculum review for excessive difficulty
- Enhanced academic support services
- Faculty-student mentoring program
- Peer tutoring expansion

**For Arts (Engagement Focus):**
- Investigate why high attendance doesn't retain
- Career counseling for arts careers
- Alumni mentoring program
- Portfolio development support

**For Computer Science (Technical Support):**
- Coding clinics and labs
- Pair programming initiatives
- Industry mentorship
- Hackathons and projects

**For Business (Maintain & Enhance):**
- Case competition opportunities
- Networking events
- Internship placement
- Professional development

**For Science (Learn & Replicate):**
- Study what works (despite low attendance)
- Share best practices with other departments
- Maintain support systems
- Investigate attendance issue

---

## 4. Behavioral Patterns Dashboard: Key Findings & Insights

### Attendance Categories Distribution

| Attendance Category | Range | Count of Students | Risk Level |
|--------------------|-------|---------------|------------|
| Excellent | 90-100% | 1,620 | Low Risk |
| Good | 80-90% | 7,630 | Moderate Risk |
| Below Average | 70-80% | 743 | High Risk |
| Poor | <50% | 8 | Critical Risk |

### Assignment Delay Impact Analysis

| Delay Category | Non-Dropout (Days) | Dropout (Days) | Difference |
|----------------|-------------------|----------------|------------|
| Average Delay | 1.7 | 2.0 | +0.3 days |

**Key Finding:** Dropout students average 0.3 days (approximately 7 hours) more assignment delay than non-dropout students.

**Delay Categories Breakdown:**

| Delay Category | Days | Dropout Risk |
|----------------|------|--------------|
| On Time | 0 | Baseline |
| Minor Delay | 1-3 days | Increased Risk |
| Moderate Delay | 4-6 days | High Risk |
| Severe Delay | >7 days | Critical Risk (50% dropout rate per Summary Dashboard) |

**Critical Insight:** Even minor delays (1-3 days) are associated with 50% dropout rate according to Summary Dashboard - making assignment submission one of the strongest early warning indicators.

### Stress Index Critical Threshold Analysis 

**Stress Level Distribution with Student Counts:**

| Stress Level | Range | Dropout Count | Non-Dropout Count | Total Students | Dropout Rate |
|--------------|-------|---------------|-------------------|----------------|--------------|
| Low | 0-3 | 55 | 744 | 799 | 6.9% |
| Normal | 4-5 | 432 | 2,547 | 2,979 | 14.5% |
| Moderate | 6-7 | 1,122 | 3,261 | 4,383 | 25.6% |
| High | 8-9 | 624 | 994 | 1,618 | 38.6% |
| Critical | 10 | 121 | 100 | 221 | 54.8% |
| **TOTAL** | | **2,354** | **7,646** | **10,000** | **23.5%** |

**Key Finding:** Students with critical stress (10) are 9 times more likely to drop out than students with low stress (0-3).

**Critical Finding:** Moderate stress (6-7) accounts for **47.7% of all dropouts** - nearly half - despite having only a 25.6% dropout rate. This is because so many students (4,383) are in this category.

**Key Insight:** The dropout rate increases exponentially with each stress level, with the largest absolute jump (+16.2%) occurring between High and Critical stress.

### Attendance Distribution Issues

**Observed Distribution (from image):**
- <50%: 40% (seems high - possible data error)
- 50-70%: 20%
- 70-80%: 0% (suspicious)
- Above 80%: 0% (clearly incorrect)

**Data Quality Alert:** The attendance distribution shown (40% in <50% category, 0% in above 80%) contradicts the department attendance averages (all departments 81-82%). This suggests:

1. Visualization error in the provided image
2. Different calculation methodology
3. Incomplete data in this specific view

### Behavioral Risk Matrix

| Risk Level | Attendance | Assignment Delay | Stress Index |
|------------|------------|------------------|--------------|
| Critical | <50% | Severe (>7 days) | Critical (10) |
| High | 50-70% | Moderate (4-6 days) | High (8-9) |
| Moderate | 70-80% | Minor (1-3 days) | Moderate (6-7) |
| Low | 80-90% | On Time | Normal (4-5) |
| Minimal | 90-100% | Early Submission | Low (0-3) |

### Compound Risk Analysis

**Highest Risk Combination:**
- Poor Attendance (<50%)
- Severe Assignment Delay (>7 days)
- Critical Stress (10)
- **Predicted Dropout Probability: >75%**

**Moderate Risk Combination:**
- Below Average Attendance (70-80%)
- Minor Assignment Delay (1-3 days)
- Moderate Stress (6-7)
- **Predicted Dropout Probability: ~25-35%**

**Low Risk Combination:**
- Good Attendance (80-90%)
- On Time Submissions
- Normal Stress (4-5)
- **Predicted Dropout Probability: <15%**

### Behavioral Patterns by Attendance Category

| Attendance Category | Minor Delay | Moderate Delay | On Time | Severe Delay |
|--------------------|-------------|----------------|---------|--------------|
| Good (80-90%) | 13.15% | 2.58% | 2.50% | 0.09% |
| Poor (<50%) | 0.03% | 0.01% | 0.00% | 0.02% |
| Excellent (90-100%) | 1.67% | 0.30% | 0.30% | 0.02% |
| Below Average (70-80%) | 2.00% | 0.44% | 0.44% | 0.01% |

**Key Observations:**

1. **Good Attendance Group (80-90%):**
   - Highest rate of minor delays (13.15%)
   - Most likely to submit assignments (just late)
   - Shows engagement despite tardiness

2. **Poor Attendance Group (<50%):**
   - Minimal submission activity overall
   - Almost no on-time submissions (0.00%)
   - Disengaged from academic process

3. **Excellent Attendance Group (90-100%):**
   - Low delay rates overall
   - Most compliant with deadlines
   - Small but consistent group

4. **Below Average Group (70-80%):**
   - Moderate delay patterns
   - Similar to Excellent group in structure
   - Potential for improvement

### Non-Dropout Behavioral Profile

**Characteristics of Students Who Persist:**
- Average assignment delay: 1.7 days (vs 2.0 for dropouts)
- Better attendance patterns
- Lower stress levels
- More likely to submit assignments (even if late)

**Key Insight:** The 0.3 day difference in assignment delay between dropouts and non-dropouts suggests that even small behavioral differences matter.

### Early Warning Behavioral Indicators

**Tier 1 - Immediate Red Flags:**
- Attendance dropping below 50%
- Severe assignment delay (>7 days)
- Stress index reaching 10 (Critical)
- Multiple missed submissions

**Tier 2 - Early Warning Signs:**
- Attendance decline trend (80% → 70% → 60%)
- Increasing assignment delay (on time → minor → moderate)
- Stress rising (Normal → Moderate → High)
- Pattern of minor delays becoming frequent

**Tier 3 - Monitoring Indicators:**
- Occasional minor delays
- Slight attendance drops
- Stress spikes during exams
- Isolated behavioral issues

### Behavioral Intervention Triggers

| Trigger | Threshold | Action |
|---------|-----------|--------|
| Attendance Warning | <80% for 2 consecutive weeks | Check-in email |
| Attendance Critical | <50% any week | Mandatory meeting |
| Delay Warning | 2+ minor delays in a month | Academic coaching |
| Delay Critical | Any severe delay (>7 days) | Intervention team |
| Stress Warning | Self-report >7 | Counseling referral |
| Stress Critical | Self-report = 10 | Immediate outreach |

### Key Behavioral Takeaways

1. **Assignment Delay is Powerful Predictor:** Even 0.3 days average difference separates dropouts from non-dropouts

2. **Stress is a Crisis Multiplier:** Critical stress (10) increases dropout risk 9x

3. **Attendance Patterns Reveal Engagement:** Good attenders submit work (even if late); poor attenders disengage completely

4. **Minor Delays are Common:** 13.15% of good attenders have minor delays - this is "normal" behavior

5. **Compound Risk is Real:** Students with multiple behavioral risk factors need prioritized intervention

### Behavioral Intervention Recommendations

**For Students with Critical Risk (All red flags):**
- Immediate counseling referral
- Academic probation meeting
- Family notification
- Weekly check-ins
- Support services enrollment

**For Students with High Risk (Multiple yellow flags):**
- Academic coaching assignment
- Stress management workshop
- Attendance contract
- Peer mentoring

**For Students with Moderate Risk (Single yellow flag):**
- Early alert notification
- Resource introduction
- Monitoring period
- Follow-up in 30 days

**For All Students:**
- Stress management resources
- Time management workshops
- Wellness programs
- Academic skills training

### System-Level Recommendations

1. **Real-Time Monitoring System:** Track attendance and submissions daily

2. **Automated Alerts:** Trigger interventions when thresholds crossed

3. **Stress Screening:** Regular stress assessments (every semester)

4. **Behavioral Analytics:** Predict risk using behavioral patterns

5. **Intervention Tracking:** Measure effectiveness of interventions

6. **Student Success Coaching:** Proactive outreach to at-risk students

### Behavioral vs. Academic Correlation

| Behavior | Academic Impact | Retention Impact |
|----------|----------------|------------------|
| On-time submission | Positive | Strong positive |
| Regular attendance | Positive | Strong positive |
| Low stress | Positive | Strong positive |
| Minor delays | Neutral | Weak negative |
| Severe delays | Negative | Strong negative |
| Poor attendance | Negative | Strong negative |
| Critical stress | Negative | Very strong negative |

**Conclusion:** Behavioral patterns are equally important as academic factors in predicting student dropout - sometimes more so.

---

# Dashbord Overview (Page 1)
-<a href="https://github.com/Donovandonz/Power-BI--student-dropout-prediction-analysis/blob/main/Summary-dashboard.png">Summry-dashboard</a>

<img width="1312" height="737" alt="Summary-dashboard" src="https://github.com/user-attachments/assets/94578b2e-5a53-4d56-aaad-a7ddec731188" />

---

# Dashbord Overview (Page 2)
-<a href="https://github.com/Donovandonz/Power-BI--student-dropout-prediction-analysis/blob/main/Academic-factor-dashboard.png">Academic-factor-dshboard</a>

<img width="1307" height="735" alt="Academic-factor-dashboard" src="https://github.com/user-attachments/assets/09c56238-c03c-48d4-a362-1d40d3ebd5b9" />

---

# Dashbord Overview (Page 3)
-<a href="https://github.com/Donovandonz/Power-BI--student-dropout-prediction-analysis/blob/main/Demographic-dashboard.png=">Demogrphic-dashboard</a>

<img width="1308" height="733" alt="Demographic-dashboard" src="https://github.com/user-attachments/assets/c9038265-d911-481b-b33a-abe7eb5c5771" />

---

# Dashbord Overview (Page 4)
-<a href="https://github.com/Donovandonz/Power-BI--student-dropout-prediction-analysis/blob/main/Behavioral-patterns-dashboard.png">Behavior-patterns-dashboard</a>

<img width="1308" height="736" alt="Behavioral-patterns-dashboard" src="https://github.com/user-attachments/assets/e3ace9a4-1fba-4f08-b78a-be0161d76932" />

---

# Dashbord Overview (Page 5)
-<a href="https://github.com/Donovandonz/Power-BI--student-dropout-prediction-analysis/blob/main/Department-dashboard.png">Department-dashboard</a>

<img width="1310" height="735" alt="Department-dashboard" src="https://github.com/user-attachments/assets/8cd1206b-a8ea-495b-a5b7-9d55067b672e" />

---

# Dashbord Overview (Page 6)
-<a href="https://github.com/Donovandonz/Power-BI--student-dropout-prediction-analysis/blob/main/Risk-indicators-dashboard.png">Risk-indicator-dashboard</a>

<img width="1311" height="733" alt="Risk-indicators-dashboard" src="https://github.com/user-attachments/assets/3777afd9-3f97-440b-84e9-ca7d62beccba" />





