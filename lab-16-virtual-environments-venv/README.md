# Lab 16: Virtual Environments (venv)

## Objective

The objective of this lab is to understand Python virtual environments and learn how to create, activate, manage, and deactivate isolated Python environments using the venv module.

---

## Lab Environment

| Component        | Details                   |
| ---------------- | ------------------------- |
| Operating System | Ubuntu Linux              |
| Python Version   | Python 3.x                |
| IDE              | PyCharm Community Edition |
| Terminal         | Ubuntu CLI                |

---

## Create Project Directory

```bash
mkdir my_project
cd my_project
```

---

## Create Virtual Environment

```bash
python3 -m venv myenv
```

### Verify

```bash
ls
```

Output:

```text
myenv
```

---

## Activate Virtual Environment

```bash
source myenv/bin/activate
```

### Example Prompt

```text
(myenv) ubuntu@server:~/my_project$
```

---

## Install a Package

```bash
pip install requests
```

---

## Verify Installed Packages

```bash
pip list
```

Example Output:

```text
Package     Version
----------- -------
requests    2.x.x
pip         xx.x.x
setuptools  xx.x.x
```

---

## Deactivate Virtual Environment

```bash
deactivate
```

---

## Key Concepts

### Virtual Environment

An isolated Python environment for a specific project.

### Isolation

Prevents dependency conflicts between different Python projects.

### Activation

```bash
source myenv/bin/activate
```

Enables the virtual environment.

### Deactivation

```bash
deactivate
```

Returns to the system Python environment.

---

## Real-World Applications

* Python development
* Data Science projects
* Web applications
* Automation scripts
* Cybersecurity tools
* SIEM integrations

---

## Screenshots

### Screenshot 1

Creating and activating the virtual environment.

### Screenshot 2

Installing requests and verifying packages using pip list.

---

## Skills Learned

* Creating virtual environments
* Activating virtual environments
* Installing project-specific packages
* Managing dependencies
* Deactivating environments
* Understanding dependency isolation

---

## Conclusion

This lab demonstrated how Python virtual environments help isolate project dependencies and maintain consistent development environments. Using venv is considered a best practice in professional Python development and significantly reduces package conflicts across projects.
