# Student Performance Analysis Dashboard 📊

This project is a beginner-friendly Power BI dashboard that analyzes student academic performance using various factors such as attendance, study hours, and internet access.

## Objective
To identify patterns and insights that influence student exam performance and visualize them using interactive dashboards.

## Dataset
The dataset contains 100 student records with the following fields:
- StudentID
- Name
- Gender
- Class
- Attendance %
- Study Hours
- Internet Access
- Exam Score
- Result (Pass/Fail)

## Tools & Technologies
- Power BI Desktop
- Microsoft Excel
- DAX (Data Analysis Expressions)

## Key Features
- KPI Cards: Total Students, Pass Count, Fail Count, Average Score
- Bar Chart: Exam scores by student
- Column Chart: Average score by study hours
- Pie Chart: Pass vs Fail distribution
- Slicers: Class and Gender

## DAX Measures Used

```DAX
Total Students = COUNT(Students[StudentID])
Pass Count = CALCULATE(COUNT(Students[StudentID]), Students[Result] = "Pass")
Fail Count = CALCULATE(COUNT(Students[StudentID]), Students[Result] = "Fail")
Average Score = AVERAGE(Students[Exam Score])
