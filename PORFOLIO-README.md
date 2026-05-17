# **1.Data Overview**

The Student Exam Performance dataset used for this exploratory is the Internal data sources, from the EIU’s Enterprise System (also called Enterprise Resource Planning Systems (ERP)).

| Attribute | Value |
| ------ | ------ |
| Number of Rows | 10000 |
| Number of Columns | 23 |
| Veracity | Structured |

**The data including these variables:**
*   student_id (int): Unique identifier for each student
*   gender (object): Student gender
*   age(int): Age of the student
*   parental_education (object): Highest education level of parents
*   family_income (object): Household income category
*   internet_access (object): Whether the student has internet access
*   study_environment (object): Quality of study environment
*   study_hours_per_day (int): Average daily study time
*   attendance_rate (int): Percentage of class attendance
*   sleep_hours (int): Average hours of sleep per night
*   social_media_hours (int): Average daily time spent on social media
*   assignment_completion_rate (int): Percentage of assignments completed by the student
*   participation_score (int): Level of student participation in class activities
*   online_courses_completed (int): Number of online courses completed by the student
*   tutoring (object): Whether the student receives additional tutoring support
*   math_score (int): Score achieved in mathematics
*   reading_score (int): Score achieved in reading
*   writing_score (int): Score achieved in writing
*   science_score (int): Score achieved in science
*   final_exam_score (int): Score achieved in the final exam
*   previous_gpa (int): Student’s GPA from previous academic periods
*   pass_fail (object): Indicates whether the student passed or failed
*   grade_category (object): Classification of overall performance (e.g., A, B, C, etc.)

The business context of this analysis is driven by the institution's need to improve educational quality and student retention. By specifying the business question, the primary goal of exploring this dataset is to identify which factors have the most significant impact on a student's final exam score and overall passing rate.

The insights generated from this data will enable the university's management to make data-driven decisions, such as providing targeted tutoring support for students who are at risk of failing.

## **2.Data Cleaning**

Prior to the analysis, the dataset was rigorously inspected for data quality issues, specifically focusing on duplicates and missing values.

**Duplicate records:** The analysis confirmed that the dataset contained no duplicate rows in its current state, ensuring each of the 10,000 observations represents a unique student record.

**Missing Values:** An inspection across all features revealed that there were 0 missing values across all 23 columns. Every feature from student IDs and demographic information to specific academic scores contained a full set of 10,000 non-null entries.

→ Because no missing values or duplicates were identified, no rows required deletion or imputation. The dataset remained consistent at 10,000 rows and 23 columns, perfectly prepared for descriptive statistical analysis.

## **3.Descriptive Statistics**

The Data Analysis tool in Excel was used to generate descriptive statistics for study hour per day, attendance rate, sleep hours and final exam score, as well as to understand the central tendency, dispersion, and overall distribution of these key academic factors. Based on the statistical output, two meaningful insights can be drawn:

<img width="602" height="191" alt="Screenshot 2026-05-17 at 10 36 07" src="https://github.com/user-attachments/assets/ca101e99-9513-491c-92b0-a39ed779599f" />

### **Insight 1: Poor Exam Performance Despite Strong Foundational Discipline**
Interestingly, while the student cohort demonstrates healthy baseline behaviors maintaining a high average attendance rate of 84.70% and an adequate 7.02 hours of sleep per night the average final exam score is concerningly low at 49.68. This discrepancy implies that the students' academic struggles are likely not caused by chronic absenteeism or sleep deprivation, but rather point to potential issues with study efficiency, study methods, or the overall difficulty of the curriculum.

The visualization reveals a wide spread of exam scores (ranging from 4.4 to 97.8) despite a relatively uniform study duration (mean of 3.02 hours, standard deviation of 1.18). This suggests that while more study hours generally correlate with higher scores, study efficiency and method likely play a more critical role in academic success than sheer study volume alone.

<img width="600" height="361" alt="Screenshot 2026-05-17 at 10 36 44" src="https://github.com/user-attachments/assets/62b4bd4c-6654-415b-96a0-fba519bb1dbb" />
                                    
> *Figure 1: Relationship between Study Hours and Final Exam Score*

### **Insight 2: The Impact of Class Attendance on Academic Outcomes**
While the descriptive statistics indicate a generally high mean attendance rate (84.70%), the figure 2 maps individual attendance percentages against the wide variance in final scores. It highlights the extent to which simply showing up to class acts as a reliable predictor of success, suggesting that while high attendance is a foundational habit, it does not automatically guarantee high scores without the accompaniment of efficient study hours.
<img width="603" height="363" alt="Screenshot 2026-05-17 at 10 37 10" src="https://github.com/user-attachments/assets/903ad117-6993-4ef3-ae2b-9bc69600bd0e" />

> *Figure 2: Relationship between Attendance Rate and Final Exam Score*
