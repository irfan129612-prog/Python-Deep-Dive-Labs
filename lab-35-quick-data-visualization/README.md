# 🧪 Lab 35: Quick Data Visualization with Matplotlib

## 📌 Lab Summary

In this lab, **Matplotlib**, one of Python's most popular data visualization libraries, was used to create a simple line chart. The graph was customized with a title and axis labels, then saved as an image file. This exercise demonstrates the fundamentals of visualizing numerical data using Python.

---

## 🎯 Objectives

- Understand the basics of data visualization using Matplotlib
- Install and configure the Matplotlib library
- Create a simple line chart
- Add chart titles and axis labels
- Save the chart as an image file

---

## 🛠️ Tools Used

- Ubuntu Linux
- Python 3.x
- Matplotlib
- PyCharm Community Edition
- Ubuntu Terminal

---

## 🗂️ Lab Environment

| Component | Details |
|----------|---------|
| Operating System | Ubuntu Linux |
| Python Version | Python 3.x |
| IDE | PyCharm Community Edition |
| Library | Matplotlib |
| Terminal | Ubuntu CLI |

---

## ✅ Task 1: Install Matplotlib

Install the Matplotlib library using pip.

```bash
pip install matplotlib
```

### Result

- ✅ Matplotlib installed successfully.

---

## ✅ Task 2: Create a Simple Line Chart

Create a Python script to plot sample data.

### Python Code

```python
import matplotlib.pyplot as plt

x = [0, 1, 2, 3, 4, 5]
y = [0, 1, 4, 9, 16, 25]

plt.plot(x, y)

plt.title("Simple Line Plot")
plt.xlabel("X Axis Label")
plt.ylabel("Y Axis Label")

plt.savefig("line_plot.png")

plt.show()
```

### Result

- ✅ A line graph was generated.
- ✅ The chart displayed correctly.
- ✅ The graph was saved as an image file.

---

## ✅ Task 3: Verify the Output

After running the script, the following image file was created:

```text
line_plot.png
```

The graph displayed:

- Line plot
- Graph title
- X-axis label
- Y-axis label

---

## 💻 Commands Used

```bash
pip install matplotlib

python3 line_plot.py
```

---

## 📋 Validation

The following tasks were successfully completed:

- ✅ Matplotlib installed
- ✅ Python script executed successfully
- ✅ Line chart generated
- ✅ Graph title added
- ✅ Axis labels displayed
- ✅ Chart saved as an image file

---

## 📚 Key Concepts

| Concept | Description |
|----------|-------------|
| Matplotlib | A Python library used for creating visualizations and charts |
| pyplot | A Matplotlib module that provides plotting functions similar to MATLAB |
| plot() | Creates a line graph from numerical data |
| title() | Adds a title to the chart |
| xlabel() | Labels the X-axis |
| ylabel() | Labels the Y-axis |
| savefig() | Saves the generated chart as an image |

---

## 🌍 Real-World Applications

Matplotlib is widely used in:

- Data Science
- Machine Learning
- Business Analytics
- Cybersecurity Dashboards
- Network Monitoring
- Security Reporting
- Trend Analysis
- Performance Monitoring

---

## 📸 Screenshots

Include screenshots for:

- Matplotlib installation
- Complete Python source code
- Generated line chart (`line_plot.png`)
- Terminal output after execution

---

## 📖 What I Learned

- How to install the Matplotlib library.
- How to create a basic line chart using Python.
- How to customize charts with titles and axis labels.
- How to save visualizations as image files.
- How data visualization helps simplify data interpretation and analysis.

---

## ✅ Conclusion

This lab introduced the fundamentals of **data visualization with Matplotlib** by creating a simple line chart from numerical data. The exercise demonstrated how Python can transform raw data into meaningful visual insights through chart customization and image export. These visualization techniques are widely used in **data science, cybersecurity dashboards, monitoring systems, and business analytics**, making Matplotlib an essential library for presenting and analyzing data effectively.
