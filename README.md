# 🎓 Student Exam Performance Analysis (NumPy Project)

## 📘 Project Description
This project analyzes student exam performance using **NumPy** to understand how study habits — such as hours studied, attendance percentage, and sleep duration — influence final exam results.  

The dataset includes details on:
- Hours studied  
- Sleep hours  
- Attendance percentage  
- Previous exam scores  
- Final exam scores  

Using **NumPy**, this project performs:
- Statistical analysis (mean, max, min, standard deviation)  
- Correlation analysis between study factors and exam performance  
- Grading system using conditional logic (`np.where()`)  
- Group-wise comparison of high vs low study/attendance/sleep groups  

**Results:**  
Students who studied more hours and maintained high attendance scored significantly better, while sleep duration showed little to no direct impact on performance.  

---

## 🧠 Objectives
- Apply **NumPy** for numerical and statistical data analysis  
- Explore relationships between student habits and exam outcomes  
- Practice conditional and logical array operations  
- Summarize analytical findings in a professional format  

---

## 🗂️ Dataset Information
**Filename:** `student_exam_scores.csv`  
**Columns:**
1. Student ID  
2. Hours Studied  
3. Sleep Hours  
4. Attendance %  
5. Previous Score  
6. Exam Score  

---

## 📊 Analysis Performed
### 1️⃣ Descriptive Statistics
Computed mean, max, min, and standard deviation for each numerical column to understand data distribution.  

### 2️⃣ Correlation Analysis
Used `np.corrcoef()` to measure relationships between:
- Hours studied and exam score  
- Attendance and exam score  
- Sleep hours and exam score  
- Previous scores and current exam performance  

### 3️⃣ Grading System
Classified students into grades (A, B, C, D, F) using `np.where()` based on their exam scores.

| Grade | Score Range | Description |
|--------|--------------|--------------|
| A | ≥ 40 | Excellent |
| B | 35–39 | Good |
| C | 30–34 | Average |
| D | 25–29 | Below Average |
| F | < 25 | Fail |

### 4️⃣ Pass/Fail Summary
- ✅ **Pass:** `exam_score ≥ 35`  
- ❌ **Fail:** `exam_score < 35`  
- Pass and Fail percentages calculated using `np.count_nonzero()`  

### 5️⃣ Group Performance Comparison
Divided students into **High** and **Low** groups for:
- Hours Studied  
- Attendance %  
- Sleep Hours  

Compared their average exam scores to find which factor had the greatest impact.

---

## 📈 Sample Insights

| Factor | High Avg | Low Avg | Difference |
|---------|-----------|----------|-------------|
| Hours Studied | 38.6 | 29.2 | +9.4 |
| Attendance % | 36.8 | 30.5 | +6.3 |
| Sleep Hours | 32.7 | 34.1 | −1.4 |

🧩 **Interpretation:**
- Students who studied more hours scored **+9.4 marks higher** on average.  
- Students with higher attendance scored **+6.3 marks higher**.  
- Sleep hours showed minimal or negative effect on marks.  

---

## 🧾 Key Findings
- **Study hours and attendance** have the strongest positive correlation with exam performance.  
- **Sleep hours** show weak correlation.  
- **76% of students passed** (Grades A–C).  
- Consistency in study time and class attendance strongly influence success.  

---

## 🛠️ Tools & Libraries
| Tool | Purpose |
|------|----------|
| **Python** | Programming Language |
| **NumPy** | Data analysis and computation |
| **CSV** | Dataset format |

---

## 📁 Project Structure
Student-Exam-Performance/
student_exam_scores.csv # Dataset file
exam_performance.py # Python analysis code
student_exam_performance_report # Full written report
README.md # GitHub project documentation
