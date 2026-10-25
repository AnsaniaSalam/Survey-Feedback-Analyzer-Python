<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:4F46E5,100:06B6D4&height=200&section=header&text=Survey%20Feedback%20Analyzer&fontSize=42&fontColor=ffffff&desc=Text%20analysis%20in%20core%20Python&descAlignY=68" alt="Survey Feedback Analyzer banner" />

![Python](https://img.shields.io/badge/Python-3.8+-3776AB?logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)
![Dependencies](https://img.shields.io/badge/dependencies-none-2EA44F)
![License](https://img.shields.io/badge/license-MIT-blue)
![Status](https://img.shields.io/badge/status-complete-success)

**A text-based feedback analysis tool built with core Python.**

</div>

---

## 📌 Overview

Survey feedback is only useful if someone can turn the comments into something readable. Going through a handful of entries by hand is easy, but it gets slow and uneven as the list grows. This project does that first pass automatically.

The feedback is kept in a dictionary of lists (serial number, name, comment, rating). The program lets the user add new entries, cleans the comments so that "Good", "GOOD" and "good!!" count as the same word, and then answers a few simple questions about the data.

---

## ✨ Features

| Feature | What it does |
|---------|--------------|
| 📥 Preloaded data | Starts with 10 feedback entries in a dictionary of lists |
| ✍️ Add your own | Takes name, feedback and a rating (1-5) from the user, with input checking |
| 🧹 Text cleaning | Removes punctuation, extra spaces and capital letters |
| 🔎 Word search | `count_word_in_feedbacks(word)` counts how many feedbacks contain a word |
| 📊 Summary | Average rating, longest comment and all unique words |
| ⭐ Sorting | Lists feedbacks from highest to lowest rating |
| 📈 Bonus | Rating spread bar chart and most used words |

---

## 🖥️ Sample Output

From a run with 12 feedbacks (10 preloaded and 2 added):

```text
Feedbacks containing "good":      3
Feedbacks containing "poor":      3
Feedbacks containing "excellent": 1

Average rating: 3.42

Longest feedback : poor response and poor handling of issue
Given by         : Kiran
Word count       : 7
Rating           : 1

Number of unique words: 37

5 star | ████ 4
4 star | ██ 2
3 star | ██ 2
2 star | ███ 3
1 star | █ 1
```

---


## 📂 Project Structure

| File | Description |
|------|-------------|
| 📓 [Survey_Feedback_Analyzer.ipynb](Survey_Feedback_Analyzer.ipynb) | The full project notebook, with all steps and saved outputs |
| 📄 [README.md](README.md) | Project overview and how to run it |
| ⚖️ [LICENSE](LICENSE) | MIT license |
---

## 🧠 How It Works

| Step | What happens |
|------|--------------|
| 1 | The 10 feedbacks are loaded into `feedback_data` |
| 2 | The user chooses how many more to add. Each one is checked and added, and serial numbers continue from 11 |
| 3 | Every comment is cleaned using `replace()`, `split()`, `join()`, `strip()` and `lower()` |
| 4 | `count_word_in_feedbacks()` counts feedbacks containing "good", "poor" and "excellent" |
| 5 | The final data, average rating, longest comment and unique words are printed |
| Extra | Feedbacks are sorted by rating with `zip()` and `sorted()` |

---

## 🛠️ Concepts Used

`dictionary of lists` · `for` and `while` loops · `if` conditions · `try` / `except` · string methods · user-defined functions · `set` · `zip()` · `sorted()` with `lambda`

---

## 🚀 Getting Started

**You need:** Python 3.8 or higher and Jupyter Notebook. No other libraries.

```bash
git clone https://github.com/YOUR-USERNAME/Survey-Feedback-Analyzer-Python.git
cd Survey-Feedback-Analyzer-Python
jupyter notebook Survey_Feedback_Analyzer.ipynb
```

Run the cells from top to bottom. Step 2 asks for input, so type your answers in the box under that cell. Enter `0` to skip adding feedbacks.

---

## 🔮 Future Improvements

- Read feedback from a CSV file instead of typing it in
- Mark each feedback as positive or negative using the rating
- Plot the rating spread with `matplotlib`

---

## 👩‍💻 Author

**Ansania Salam**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Ansania%20Salam-0A66C2?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ansania-salam)

---

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:06B6D4,100:4F46E5&height=100&section=footer" alt="footer" />
