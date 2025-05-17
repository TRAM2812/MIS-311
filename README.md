# MIS-311

**Part 1: Data Analysis and Insight**

**Context and Objective**

This project investigates the relationship between students' academic performance and demographic factors, with a specific focus on race/ethnicity, gender  and parental level of education. The dataset was sourced from 06_Student Performance.xlsx, providing valuable insights into student test results and background characteristics.

The dataset contains 203 rows and 8 columns, including scores in math, reading, and writing, as well as total score, average score, and key demographic variables such as race/ethnicity, gender, and parental level of education. These variables enable a comprehensive analysis of academic performance in relation to students' demographic backgrounds.

The main objective of this analysis is to explore how demographic factors influence academic outcomes and to identify patterns that could inform more effective educational strategies.

Key Variables

- Race/Ethnicity (object): Different racial groups of students.


- Parental Level of Education (object): The educational background of the student's family.


- Math Score (int): Student’s performance in math.


- Reading Score (int): Student’s performance in reading.


- Writing Score (int): Student’s performance in writing skills.

**Data Cleaning**
The dataset was first examined for missing values and duplicate rows.

**Missing Value**: Two columns were found to contain the missing value.

- Parental Level of Education had 3 missing entries. To handle this, a pivot table was created to determine the most frequently occurring education level. The mode was "associate's degree" which appeared 51 times, so this value was used to fill in the missing values.
  
- The Average Score column had 4 missing values. Since the Average Score is a derived value (calculated from Math, Reading, and Writing scores), these missing values were filled using the formula: Average Score = (Math Score + Reading Score + Writing Score) / 3. This ensured that the calculated values accurately reflected the students’ overall performance.

**Duplicates:**
There were 3 duplicate rows in the dataset. These were removed by using Excel’s “Remove Duplicates” feature under the Data Tools tab.

**Descriptive Statistics**

![image](https://github.com/user-attachments/assets/fde76eb0-9269-4ee1-8ba0-1af51720d439)

Figure 1: Average Score for Each Subject by Parental Level of Education

- Higher parental education levels are associated with higher student performance: The chart clearly shows that students whose parents have a master’s degree achieve the highest average scores across all three subjects: Math (68), Reading (75), and Writing (74). On the other hand, students whose parents only completed some high school have the lowest scores: Math (59), Reading (62), and Writing (60). This suggests a strong correlation between parents’ education levels and students’ academic success.

- Reading scores consistently outperform math and writing scores at all education levels: At every parental education level, the average reading score is either the highest or equal to the highest among the three subjects. For instance, among students with parents holding a bachelor’s degree, the reading and writing scores are both 74, higher than the math score of 71. This may indicate that reading skills are generally stronger or better supported at home, regardless of the parents' education level.

![image](https://github.com/user-attachments/assets/5c779165-674b-4e57-aea4-1c2edf227907)

Figure 2: Average Score in Writing, Reading, and Math by Gender

- Gender 0 has higher average scores than Gender 1 in all three subjects.
According to the chart, students in Group 0 outperform those in Gender 1 across all subjects. Specifically, Gender 0 scores 71.90 in writing, 72.45 in reading, and 63.57 in math. In comparison, Group 1 scores  60.89 in writing, 62.85 in reading, and 64.86 in math. The performance gap is especially noticeable in writing and reading, where Gender 0 leads by around 10-11 points. This suggests a significant difference in academic performance between the two groups.

- Each group of gender shows strength in a different subject, Gender 0 excels in writing, while Gender 1 performs best in math.
Gender 0 achieves its highest average score in reading (72.45), indicating strong reading skills. On the other hand, Gender 1 highest score is in math (62.85), which surpasses its reading (60.89) and writing (64.86) scores. This reveals that the two groups may have different academic strengths: Gender 0 tends to perform better in expressive subjects like reading, whereas Gender 1 shows stronger performance in logical and analytical areas like math.

**Conclusion and Implications**

The analysis reveals demographic factors particularly parental level of education and gender that have a significant impact on students' academic performance. By comparing the average scores across different groups, clear patterns emerge, indicating that a student’s background can influence their ability to perform well in certain subjects.

These findings highlight the importance of creating more equitable and targeted educational strategies. Schools and educators might consider offering additional academic support to students from less advantaged backgrounds or designing subject-specific tutoring programs based on the performance trends identified. Understanding the relationship between background factors and academic outcomes can help build a more inclusive learning environment that better supports all students.
