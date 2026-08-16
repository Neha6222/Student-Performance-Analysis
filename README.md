# Student Performance Analysis

## 📌 Project Overview

This is a beginner-level Python data analysis project that demonstrates how to analyze student marks using **Pandas, NumPy, Matplotlib, and Seaborn**.

The project creates a small student dataset, calculates total and average marks, assigns student ranks based on total marks, and visualizes average performance using a bar chart.

## 🎯 Objectives

* Create and structure student performance data using Pandas.
* Calculate total marks across subjects.
* Calculate average marks for each student.
* Rank students based on their total marks.
* Display and inspect the processed dataset.
* Visualize students' average marks using Matplotlib.

## 🛠️ Technologies Used

* **Python**
* **NumPy**
* **Pandas**
* **Matplotlib**
* **Seaborn**
* **Jupyter Notebook**

## 📊 Dataset

The project uses a small manually created dataset containing student marks in three subjects:

* Mathematics
* Science
* Social Studies

The dataset contains **5 students**.

## 🔍 Analysis Performed

### 1. Dataset Creation

A Pandas DataFrame is created containing student names and their subject-wise marks.

### 2. Total Marks

Total marks are calculated by adding the marks obtained in Mathematics, Science, and Social Studies.

```python
df['Total'] = df['Maths'] + df['Science'] + df['Social']
```

### 3. Average Marks

Average marks are calculated using the total marks divided by the number of subjects.

```python
df['Average'] = df['Total'] / 3
```

### 4. Student Ranking

Students are ranked according to their total marks, with the highest total receiving Rank 1.

```python
df['Rank'] = df['Total'].rank(ascending=False)
```

### 5. Data Visualization

A bar chart is created to compare the average marks of the students.

The visualization helps quickly identify differences in overall academic performance.

## 📈 Results

| Student | Total Marks | Average | Rank |
| ------- | ----------: | ------: | ---: |
| Neha    |         294 |   98.00 |    1 |
| Priya   |         245 |   81.67 |    2 |
| Pandu   |         239 |   79.67 |    3 |
| Pinky   |         236 |   78.67 |    4 |
| Sonu    |         215 |   71.67 |    5 |

### Key Observation

**Neha** achieved the highest total and average marks, resulting in Rank 1.

**Sonu** had the lowest total and average marks among the five students.

## 📁 Repository Structure

```text
Student-Performance-Analysis/
│
├── Python/
│   ├── Student_Performance_Analysis.ipynb
│   └── README.md
│
├── README.md
│
└── requirements.txt
```

## 🚀 How to Run

Install the required dependencies:

```bash
pip install -r requirements.txt
```

Open the notebook:

`Python/Student_Performance_Analysis.ipynb`

The notebook can be executed using **Jupyter Notebook, JupyterLab, or Google Colab**.

## 🎯 Project Outcome

This project demonstrates fundamental Python data-analysis skills, including:

* DataFrame creation
* Data manipulation
* Column calculations
* Ranking
* Descriptive analysis
* Data visualization

## 👩‍💻 Author

**Neha Priya**

**Skills:** Python | Pandas | NumPy | Matplotlib | Seaborn
