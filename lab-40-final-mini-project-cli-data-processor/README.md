# Lab 40: Final Mini-Project - CLI Data Processor

## Objective

The objective of this mini-project is to build a command-line Python application that fetches JSON data from an API, validates the response, logs progress, handles errors, and saves the data into a JSON file.

---

## Lab Environment

| Component        | Details                   |
| ---------------- | ------------------------- |
| Operating System | Ubuntu Linux              |
| Python Version   | Python 3.x                |
| IDE              | PyCharm Community Edition |
| Terminal         | Ubuntu CLI                |

---

## Features

* Fetch data from an API
* Parse JSON response
* Save JSON data to a file
* Accept command-line arguments
* Log program progress
* Handle HTTP and request errors
* Validate JSON response

---

## Complete Code

```python
import argparse
import json
import logging
import requests


logging.basicConfig(
    level=logging.INFO,
    format="%(asctime)s - %(levelname)s - %(message)s"
)


def fetch_data(api_url):
    try:
        response = requests.get(api_url)
        response.raise_for_status()
        data = response.json()
        return data

    except requests.exceptions.HTTPError as http_err:
        logging.error(f"HTTP error occurred: {http_err}")

    except requests.exceptions.RequestException as req_err:
        logging.error(f"Request error occurred: {req_err}")

    except ValueError:
        logging.error("Invalid JSON response received.")

    return None


def save_data_to_file(data, file_path):
    try:
        with open(file_path, "w") as json_file:
            json.dump(data, json_file, indent=4)

        logging.info(f"Data successfully saved to {file_path}")

    except Exception as error:
        logging.error(f"Error saving data: {error}")


def parse_arguments():
    parser = argparse.ArgumentParser(
        description="CLI Data Processor"
    )

    parser.add_argument(
        "--api_url",
        type=str,
        required=True,
        help="API URL to fetch data from"
    )

    parser.add_argument(
        "--file_path",
        type=str,
        required=True,
        help="Path to save JSON data"
    )

    return parser.parse_args()


if __name__ == "__main__":
    args = parse_arguments()

    logging.info("Started fetching data...")

    data = fetch_data(args.api_url)

    if data:
        save_data_to_file(data, args.file_path)
    else:
        logging.error("No data saved.")
```

---

## Run Command

```bash
python3 data_processor.py --api_url https://api.github.com --file_path github_data.json
```

---

## Output

```text
INFO - Started fetching data...
INFO - Data successfully saved to github_data.json
```

---

## Generated File

```text
github_data.json
```

---

## Key Concepts

### CLI Application

A command-line tool that accepts user input through terminal arguments.

### requests

Used to send HTTP GET requests to APIs.

### JSON

Used to store and exchange structured data.

### argparse

Used to parse command-line arguments.

### logging

Used to monitor program execution.

### Exception Handling

Prevents crashes and handles errors gracefully.

---

## Real-World Applications

* API data collection
* Automation tools
* Data pipelines
* Security intelligence scripts
* GitHub API integrations
* SIEM data processing

---

## Screenshots

**Screenshot 1:** Complete source code

**Screenshot 2:** Terminal output and generated JSON file

---

## Skills Learned

* Fetching API data
* Saving JSON files
* Building CLI tools
* Using argparse
* Implementing logging
* Handling exceptions
* Validating JSON responses

---

## Conclusion

This final mini-project combined multiple Python concepts into one practical CLI application. The project demonstrated how to fetch API data, validate JSON, save output to a file, and monitor progress through structured logging. This type of tool is useful in automation, data processing, and cybersecurity workflows.
