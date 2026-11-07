📊 Pandas Series and DataFrame Using Python

📌 Project Overview

This project demonstrates the fundamentals of data analysis using Python and the Pandas library.

The program uses two important Pandas data structures: Series and DataFrame.

It creates a Series to store student marks and a DataFrame to organize student information, including roll numbers, names, departments, and marks.

The program also performs basic data analysis by calculating average marks and filtering students based on their scores.

🎯 Objectives

- Understand Pandas Series and DataFrame.
- Store and organize student information.
- Perform basic statistical calculations.
- Calculate the average marks of students.
- Filter students based on specified conditions.
- Learn fundamental data analysis techniques using Python.

🛠️ Technologies Used

- Programming Language: Python
- Library: Pandas
- Development Environment: Visual Studio Code
- Concepts: Data Analysis, Series, DataFrame, Data Filtering

✨ Features

1. Pandas Series

Creates a one-dimensional labeled array containing student marks.

2. Pandas DataFrame

Organizes student information into rows and columns.

3. Average Mark Calculation

Calculates the average marks of all students using the "mean()" function.

4. Student Data Filtering

Displays students who scored more than 85 marks.

5. Structured Data Representation

Presents student information in an organized tabular format.

💻 Source Code

import pandas as pd

marks = pd.Series(
    [85, 91, 78, 88, 95],
    index=["A", "B", "C", "D", "E"]
)

print("--- Pandas Series ---")
print(marks)

data = {
    "RollNo": [101, 102, 103, 104, 105],
    "Name": ["Anitha", "Bala", "Chitra", "Dinesh", "Ezhil"],
    "Department": ["CSE", "CSE", "ECE", "CSE", "ECE"],
    "Mark": [85, 91, 78, 88, 95]
}

df = pd.DataFrame(data)

print("\n--- DataFrame ---")
print(df)

print("\nAverage Mark:", round(df["Mark"].mean(), 2))

print("\nStudents scoring above 85:")
print(df[df["Mark"] > 85])

📊 Sample Output

--- Pandas Series ---
A    85
B    91
C    78
D    88
E    95
dtype: int64

--- DataFrame ---
   RollNo    Name Department  Mark
0     101  Anitha        CSE    85
1     102    Bala        CSE    91
2     103  Chitra        ECE    78
3     104  Dinesh        CSE    88
4     105   Ezhil        ECE    95

Average Mark: 87.4

Students scoring above 85:
   RollNo    Name Department  Mark
1     102    Bala        CSE    91
3     104  Dinesh        CSE    88
4     105   Ezhil        ECE    95

⚙️ Installation and Execution

Step 1: Install Python

Ensure Python is installed on your computer.

Step 2: Install Pandas

Open the terminal in Visual Studio Code and execute:

python -m pip install pandas

Step 3: Save the Program

Save the Python program as:

main.py

Step 4: Run the Program

Execute the following command:

python main.py

🔍 Working Principle

Step 1: Import Pandas

The Pandas library is imported using "import pandas as pd".

Step 2: Create a Series

A Pandas Series is created to store student marks with custom labels.

Step 3: Create a DataFrame

Student details are stored in a Python dictionary and converted into a Pandas DataFrame.

Step 4: Calculate Average Marks

The "mean()" function calculates the average marks of all students.

Step 5: Filter Student Records

Boolean indexing is used to identify students scoring above 85 marks.

Step 6: Display Results

The program displays the Series, DataFrame, average marks, and filtered student records.

🌍 Applications

- Student Performance Analysis
- Educational Data Management
- Academic Record Processing
- Data Science Fundamentals
- Statistical Data Analysis
- Data Filtering and Reporting

🚀 Future Enhancements

- Import student records from CSV files.
- Export analyzed data to Excel.
- Visualize student performance using Matplotlib.
- Calculate department-wise average marks.
- Identify top-performing students.
- Develop an interactive student performance dashboard.

📚 Learning Outcomes

Through this project, I gained practical experience in:

- Creating and manipulating Pandas Series.
- Working with Pandas DataFrames.
- Organizing structured datasets.
- Performing statistical calculations.
- Filtering records using Boolean conditions.
- Understanding fundamental data analysis operations.

👨‍💻 Author

KARTHICK B

Computer Science and Engineering
Chennai Institute of Technology

📄 Conclusion

This project demonstrates the fundamental concepts of data handling and analysis using Python and Pandas.

By implementing Series, DataFrames, statistical calculations, and conditional filtering, the program provides a foundation for more advanced data analysis and data science applications.