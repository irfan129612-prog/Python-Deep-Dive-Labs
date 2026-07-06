# Lab 23: Using Requests for HTTP Calls

## Objective

The objective of this lab is to understand how to perform HTTP requests using Python's requests library, interpret status codes, and parse JSON data returned by web APIs.

---

## Lab Environment

| Component        | Details                   |
| ---------------- | ------------------------- |
| Operating System | Ubuntu Linux              |
| Python Version   | Python 3.x                |
| IDE              | PyCharm Community Edition |
| Terminal         | Ubuntu CLI                |

---

## Install Requests Library

```bash
pip install requests
```

---

## Complete Code

```python
import requests

response = requests.get("https://api.github.com")

print("Status Code:", response.status_code)

response_data = response.json()

print("\nGitHub API Response:")
print(response_data)

print("\nCurrent User URL:", response_data["current_user_url"])
print("Repository URL:", response_data["repository_url"])
```

---

## Example Output

```text
Status Code: 200

Current User URL:
https://api.github.com/user

Repository URL:
https://api.github.com/repos/{owner}/{repo}
```

---

## Key Concepts

### HTTP Request

A request sent from a client to a server.

### GET Request

Used to retrieve information from a server.

```python
requests.get(url)
```

### Status Code

Indicates the result of an HTTP request.

| Code | Meaning      |
| ---- | ------------ |
| 200  | Success      |
| 404  | Not Found    |
| 500  | Server Error |

### JSON

A lightweight data-interchange format commonly used by APIs.

### response.json()

Converts JSON data into a Python dictionary.

---

## Real-World Applications

* GitHub API
* Wazuh API
* VirusTotal API
* Shodan API
* Cloud APIs
* Web Automation

---

## Screenshots

### Screenshot 1

Complete source code.

### Screenshot 2

Program output showing status code and API data.

---

## Skills Learned

* Installing requests
* Making HTTP GET requests
* Reading HTTP status codes
* Parsing JSON responses
* Accessing API data
* Understanding REST APIs

---

## Conclusion

This lab demonstrated how to interact with web APIs using Python's requests library. HTTP requests were sent successfully, status codes were interpreted, and JSON responses were converted into Python dictionaries for further processing.
