# Data Formatting Issues

---

# Data

- Numbers, names, dates, …
- Graphs, images, …
- Organised in tables,  list, ...
- Popular file formats:  `.txt`, `.csv`, `.xls`

---

# 1st Rule

- Always, always **RAW** data
- NOT 
    + processed, 
    + filtered 
    + manipulated 
    + either electronically or manually

---

# 1st Rule - Why?

- Maintain consistency
    + Data format
    + Codes (M/F)
    + Separator , ; \t
- Reduce human errors
    + Copy / Paste / Cut
    + Deletion
Addition unwanted characters
- Reduce machine errors
    + Cell formats
    + Save file with a different extension

---

# 2nd Rule - Maintain consistency

---

# Example 1

| Patient ID | Sex    | Date of birth     |
|------------|--------|-------------------|
| 1          | M      | 01-01-2013        |
| 2          | f      | 04-18-1998        |
| 3          | Male   | 1st of April 2004 |
| 4          | Female | NA                |
| 5          | F      | 2010/03/12        |
| 6          | F      |                   |
| 7          | M      | 10012012          |

---

# Example 1

- Consistency: F, female, f, fem, 2, …
- Single common format for all dates: YYYYMMDD, YYYY-MM-DD
    + http://www.iso.org/iso/home/standards/iso8601.htm
- Consistency about missing values
    + NA (not available), NULL,     , ...

---

# Example 1 - corrected

| Patient ID | Sex  | Date of birth |
|------------|------|---------------|
| 1          | M    | 2013-01-01    |
| 2          | F    | 1998-04-18    |
| 3          | M    | 2004-04-01    |
| 4          | F    | NA            |
| 5          | F    | 2010-03-12    |
| 6          | F    | NA            |
| 7          | M    | 2012-01-10    |

---

# A bit more about consistency

- Realistic and easy to understand
    + Variable names
    + File names
- Unique and consistent variable names
    + Multiple tables
    
---

# 3rd Rule

## Missing values = NA

---

# Blank spaces

- Careful!!!

- Blank cell ≠ space
- “Male” ≠ “ Male “
- Last line: “ “ 
    + These can be a headache later on!

---

# Example 2

| Patient ID | Date       | Value |
|------------|------------|-------|
| 1          | 2015-06-14 | 213   |
| 2          |            | 76.5  |
| 3          | 2015-06-18 | 32    |
| 4          |            | 120.3 |
| 5          |            | 109   |
| 6          | 2015-06-20 |       |
| 7          |            | 143   |

---

# Example 2

- It is tempting to make the table look cleaner by not repeating some values
- Fill in all cells!
    + Problems when sorting
- Empty cell:
    + Missing value?
    + Value meant to be repeated multiple times?
- Make sure it’s clear that the data is missing and not unintentionally left blank

---

# Example 2 Corrected

| Patient ID | Date       | Value |
|------------|------------|-------|
| 1          | 2015-06-14 | 213   |
| 2          | 2015-06-14 | 76.5  |
| 3          | 2015-06-18 | 32    |
| 4          | 2015-06-18 | 120.3 |
| 5          | 2015-06-18 | 109   |
| 6          | 2015-06-20 |       |
| 7          | 2015-06-20 | 143   |

---

# Rule 4

## Make it rectangle

