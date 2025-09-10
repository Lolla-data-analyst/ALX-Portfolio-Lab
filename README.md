# Student Admission System - Pseudocode Implementation

## 📋 Project Overview

This project implements a pseudocode solution for determining student admission to ALX Academy's Data program based on examination results. The system evaluates students across four subjects and applies specific admission criteria.

## 🎯 Problem Statement

The admission committee of ALX Academy was tasked with admitting students into the Data program.

**Examination Subjects:**
- English
- Mathematics  
- Physics
- Chemistry

**Admission Criteria:**
To be admitted into the data program, a student must:
- Pass English **AND** Mathematics (both mandatory)
- Pass Physics **OR** Chemistry (at least one required)

**Example:** If a student passed English, Math, and Chemistry but failed Physics, they would still be admitted because passing English and Math is compulsory while they just need to pass either Physics or Chemistry.

## 💻 Pseudocode Solution

```
Start
    Read English, Mathematics, Physics, Chemistry
    IF(English == Pass AND Mathematics == Pass) then
        IF (Physics == Pass OR Chemistry == Pass) Then
            Output "Admitted"
        Else
            Output "Not Admitted"
        End If
    Else
        Output "Not Admitted"
    End If
End
```

## 🔍 Logic Explanation

The pseudocode uses a nested conditional structure:

1. **First Check:** Verify if both English and Mathematics are passed
   - If either fails → Student is not admitted
   - If both pass → Proceed to second check

2. **Second Check:** Verify if at least one science subject is passed
   - If Physics OR Chemistry is passed → Student is admitted
   - If both science subjects fail → Student is not admitted

## 📊 Testing & Implementation

### Dataset
- Created a test dataset with 25+ student records
- Each record contains scores for all four subjects
- Applied the admission logic using spreadsheet formulas

### Excel/Google Sheets Formula
```excel
=IF(AND(B2>=60, C2>=60, OR(D2>=60, E2>=60)), "Admitted", "Not Admitted")
```

Where:
- Column B: English scores
- Column C: Mathematics scores  
- Column D: Physics scores
- Column E: Chemistry scores
- Pass mark: 60

## 📁 Repository Contents

```
├── README.md                 # Project documentation
├── student_data.csv         # Test dataset with student scores
├── pseudocode.txt           # Raw pseudocode file
└── screenshots/             # Results and implementation images
    └── spreadsheet_results.png
```

## 🚀 How to Use

1. **Download the dataset:** `student_data.csv`
2. **Import to spreadsheet:** Excel, Google Sheets, etc.
3. **Apply the formula:** Use the provided Excel formula in column F
4. **Verify results:** Check admission decisions against the pseudocode logic

## 🎓 Learning Outcomes

This project demonstrates:
- **Logical thinking:** Breaking down complex admission criteria into simple conditions
- **Pseudocode writing:** Translating business rules into algorithmic steps
- **Conditional logic:** Using nested IF statements and boolean operators
- **Data validation:** Testing logic against real datasets

## 📈 Part of Learning Journey

This project is part of my **#166daysofBecoming** challenge, specifically from the ALX Portfolio Lab sessions where we practice problem-solving and algorithmic thinking.

**Day 39 of 166 days of Becoming**

---

## 🔗 Connect with Me

- **LinkedIn:** [[My LinkedIn profile](https://www.linkedin.com/in/mercy-adegunju/)]
- **Portfolio:** [On It.]

## 📝 License

This project is for educational purposes as part of the ALX Data Science program.

---

*#ALXprojectportfolio #DataScience #ProblemSolving #Pseudocode*
