# MiniProject — Student Marks Analyzer

A small C++ console program that reads marks for a group of students and prints a summary report.

## Features

- Reads the number of students (1–100)
- Reads each student's mark
- Prints a report with:
  - Total and average marks
  - Highest and lowest marks
  - Number of students who passed (mark ≥ 40) and failed
- Lets you analyze another group without restarting (`y` / `n`)

## Requirements

- A C++ compiler such as `g++` (e.g. MSYS2 UCRT64 on Windows)

## Build and run

```sh
g++ -Wall -o program program.cpp
./program
```

On Windows (PowerShell):

```powershell
g++ -Wall -o program.exe program.cpp
.\program.exe
```

## Example

```
============================
   STUDENT MARKS ANALYZER
============================
Enter number of students: 3
Enter mark of student 1: 45
Enter mark of student 2: 78
Enter mark of student 3: 90

========== STUDENT REPORT ==========
Total Marks  : 213
Average      : 71
Highest Mark : 90
Lowest Mark  : 45
Passed       : 3
Failed       : 0
====================================

Do you want to analyze again? (y/n): n

Thank you for using Student Marks Analyzer!
```

## Program structure

| Function        | Purpose                                      |
|-----------------|----------------------------------------------|
| `readMarks`     | Reads each student's mark                    |
| `findTotal`     | Sums all marks                               |
| `findAverage`   | Returns the average mark                     |
| `findHighest`   | Returns the highest mark                     |
| `findLowest`    | Returns the lowest mark                      |
| `countPassed`   | Counts students with a mark of 40 or more    |
| `printReport`   | Prints the summary report                    |
| `main`          | Shows the menu and repeats until you answer `n` |
