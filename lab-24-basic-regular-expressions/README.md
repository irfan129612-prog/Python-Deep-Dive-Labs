# Lab 24: Basic Regular Expressions

## Objective

The objective of this lab is to understand regular expressions (regex) in Python, perform pattern matching, replace text, and extract structured information using groups.

---

## Lab Environment

| Component        | Details                   |
| ---------------- | ------------------------- |
| Operating System | Ubuntu Linux              |
| Python Version   | Python 3.x                |
| IDE              | PyCharm Community Edition |
| Terminal         | Ubuntu CLI                |

---

## Complete Code

```python
import re

pattern = re.compile(r"\d+")

test_string = "The rainfall 2021 was greater than 2019 and 2020 combined."

matches = pattern.findall(test_string)

print("Matches Found:", matches)

replaced_string = pattern.sub("XXXX", test_string)

print(replaced_string)

date_pattern = re.compile(r"(\d{4})-(\d{2})-(\d{2})")

date_string = "Date of birth: 1990-08-15 and starting date 2020-01-01."

date_matches = date_pattern.findall(date_string)

print(date_matches)

named_date_pattern = re.compile(
    r"(?P<year>\d{4})-(?P<month>\d{2})-(?P<day>\d{2})"
)

for match in named_date_pattern.finditer(date_string):

    print(
        match.group("year"),
        match.group("month"),
        match.group("day")
    )
```

---

## Output

```text
Matches Found: ['2021', '2019', '2020']

Replaced String:
The rainfall XXXX was greater than XXXX and XXXX combined.

Date Matches:
[('1990', '08', '15'), ('2020', '01', '01')]
```

---

## Key Concepts

### Regular Expression

A pattern used for searching and matching text.

### \d

Matches a digit.

### +

Matches one or more occurrences.

### findall()

Returns all matches.

### sub()

Replaces matched text.

### Groups

Captures parts of a pattern using parentheses.

### Named Groups

Allows groups to be referenced by name.

---

## Real-World Applications

* SIEM log analysis
* Email extraction
* IP address detection
* URL parsing
* CVE extraction
* Data cleaning

---

## Screenshots

### Screenshot 1

Complete source code.

### Screenshot 2

Program output.

---

## Skills Learned

* Using the re module
* Compiling regex patterns
* Finding matches
* Replacing text
* Using groups
* Using named groups

---

## Conclusion

This lab demonstrated how regular expressions can efficiently search, extract, and manipulate text. Regex is a critical skill in Data Science, Automation, and Cybersecurity, especially for log analysis and pattern matching tasks.
