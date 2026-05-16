# 📊 Student Exam Performance Analysis Portfolio

## 1. Data Overview
The dataset contains a comprehensive set of variables designed to evaluate student performance, including:
*   `study_hours_per_day`: Average daily study time.
*   `attendance_rate`: Percentage of class attendance.
*   `sleep_hours`: Average hours of sleep per night.
*   `final_exam_score`: Score achieved in the final exam.
*   `pass_fail`: Indicates whether the student passed or failed.
*   `grade_category`: Student's letter grade classification (A, B, C, etc.).

## 2. Data Cleaning
Prior to analysis, the dataset underwent rigorous data cleaning procedures to handle any inconsistencies, missing values, or duplicate records, ensuring the dataset was completely valid and consistent for statistical analysis.

## 3. Descriptive Statistics
The following table summarizes the central tendencies and dispersion of the four core academic metrics:

| Metric | Mean | Median | Mode | Std. Dev | Minimum | Maximum |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **Study Hours/Day** | 3.02 | 3.00 | 3.00 | 1.18 | 1.00 | 5.00 |
| **Attendance Rate (%)** | 84.70 | 85.00 | 85.00 | 9.99 | 60.00 | 100.00 |
| **Sleep Hours/Night** | 7.02 | 7.00 | 7.00 | 1.00 | 5.00 | 9.00 |
| **Final Exam Score** | 49.68 | 49.30 | 31.80 | 19.19 | 4.40 | 97.80 |

## 4. Key Insights

### 💡 Insight 1: Poor Exam Performance Despite Strong Foundational Discipline
Interestingly, while the student cohort demonstrates healthy baseline behaviors—maintaining a high average attendance rate of 84.70% and an adequate 7.02 hours of sleep per night—the average final exam score is concerningly low at 49.68. This discrepancy implies that the students' academic struggles are likely not caused by chronic absenteeism or sleep deprivation, but rather point to potential issues with study efficiency, study methods, or the overall difficulty of the curriculum. The massive variance in exam scores (from 4.4 to 97.8) against a relatively uniform study duration (approx. 3 hours) further emphasizes that study *quality* heavily outweighs study *quantity*.

### 💡 Insight 2: The True Impact of Class Attendance
While attendance is a strong foundational habit, visualizing the relationship between attendance rates and final exam scores reveals that simply showing up to class does not automatically guarantee high marks. The data indicates that high attendance acts as a reliable predictor of success only when accompanied by effective, independent study habits.

## 5. Visualizations
The analysis is supported by the following visualizations:
1.  **Scatter Plot:** Relationship between Study Hours and Final Exam Score.
2.  **Scatter Plot:** Relationship between Attendance Rate and Final Exam Score.
