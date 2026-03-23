# TuTeDude Assignment 2 – Python and Bash Grade Checker

## 📌 Task
Write a program that takes a score as input and prints the grade:
- 90 and above → A
- 80–89 → B
- 70–79 → C
- 60–69 → D
- Below 60 → F

---

## 🐍 Python Solution (`grade_checker.py`)
```python
score = int(input("Enter your score: "))

if score >= 90:
    print("Grade: A")
elif score >= 80:
    print("Grade: B")
elif score >= 70:
    print("Grade: C")
elif score >= 60:
    print("Grade: D")
else:
    print("Grade: F")

Example Run:
Enter your score: 85
Grade: B

Bash Solution (grade_checker.sh)

#!/bin/bash
read -p "Enter your score: " score

if [ $score -ge 90 ]; then
    echo "Grade: A"
elif [ $score -ge 80 ]; then
    echo "Grade: B"
elif [ $score -ge 70 ]; then
    echo "Grade: C"
elif [ $score -ge 60 ]; then
    echo "Grade: D"
else
    echo "Grade: F"
fi


Example Run:

$ ./grade_checker.sh
Enter your score: 72
Grade: C



## 📂 Repository Structure
TuTeDude_Assignment-1_Python-and-Bash-Grade-Checker/
│
├── grade_checker.py   # Python solution
├── grade_checker.sh   # Bash solution
└── README.md          # Documentation

