# Student Data Analysis (Plain Python)

This version reads a file of students and works out how many male and female students there are, and the average grade point average (GPA) for each. It uses only plain Python, with no extra libraries.

## Before you start

You need Python 3 and Jupyter Notebook (or VS Code with the Jupyter extension). There is nothing else to install.

## Your data file

The data is in `students-data.csv`, included in this branch. It has a header row, then one student per line. Two columns are used:

- **gender**, the third column (`male` or `female`)
- **GPA**, the fifth column

```csv
ID,class,gender,race,GPA,...
1141,A,male,1,73.47,...
1142,A,female,1,71.22,...
```

To use your own file, change `FILE_PATH` at the top of the notebook.

## How to run

1. Open `Student-Data-Analysis.ipynb`.
2. Run the cell.

## Example output

```text
Male students: 37
Female students: 68
Average male grade point average: 81.85
Average female grade point average: 83.56
```

## How it works

The program goes through the students one at a time. For each one it adds 1 to the count for their gender and adds their GPA to that gender's total. At the end, total divided by count gives the average.
