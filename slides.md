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
