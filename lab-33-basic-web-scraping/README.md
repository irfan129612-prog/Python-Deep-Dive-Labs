# Lab 33: Basic Web Scraping with requests and BeautifulSoup

## Objective

The objective of this lab is to understand the fundamentals of web scraping using Python's requests and BeautifulSoup libraries, retrieve web pages, parse HTML content, and extract useful information.

---

## Lab Environment

| Component        | Details                   |
| ---------------- | ------------------------- |
| Operating System | Ubuntu Linux              |
| Python Version   | Python 3.x                |
| IDE              | PyCharm Community Edition |
| Terminal         | Ubuntu CLI                |

---

## Install Required Packages

```bash
pip install requests beautifulsoup4
```

---

## Complete Code

```python
import requests
from bs4 import BeautifulSoup

response = requests.get("https://example.com")

print("Status Code:", response.status_code)

soup = BeautifulSoup(
    response.text,
    "html.parser"
)

title = soup.title.string

print("Page Title:", title)

links = soup.find_all("a")

for link in links:
    print(link.get("href"))
```

---

## Output

```text
Status Code: 200

Page Title:
Example Domain

Links Found:
https://www.iana.org/domains/example
```

---

## Key Concepts

### HTTP Request

Retrieves webpage content.

```python
requests.get()
```

### Status Code

Indicates success or failure of the request.

### BeautifulSoup

Parses HTML documents.

### HTML Parsing

Extracts specific elements from webpages.

### find_all()

Finds all matching HTML tags.

### href

Contains hyperlink URLs.

---

## Real-World Applications

* Data collection
* News aggregation
* Price monitoring
* Job scraping
* Security intelligence gathering
* Threat intelligence collection

---

## Screenshots

### Screenshot 1

Complete source code.

### Screenshot 2

Program output.

---

## Skills Learned

* Installing BeautifulSoup
* Making HTTP requests
* Parsing HTML
* Extracting page titles
* Extracting hyperlinks
* Basic web scraping

---

## Conclusion

This lab demonstrated the basics of web scraping using Python. By combining requests and BeautifulSoup, students can retrieve web content, navigate HTML structures, and extract valuable information for automation, analytics, and cybersecurity projects.
