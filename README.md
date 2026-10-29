
# Python-For-Data-Science
=======
# Python for Data Science 🚀

[![Python Version](https://img.shields.io/badge/python-3.10%20%7C%203.11%20%7C%203.12%20%7C%203.13-blue.svg)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebooks-orange?logo=jupyter)](https://jupyter.org/)
[![NumPy](https://img.shields.io/badge/NumPy-1.26+-013243?logo=numpy)](https://numpy.org/)
[![Pandas](https://img.shields.io/badge/Pandas-2.0+-150458?logo=pandas)](https://pandas.pydata.org/)
[![Scikit-Learn](https://img.shields.io/badge/scikit--learn-1.4+-F7931E?logo=scikit-learn)](https://scikit-learn.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](#license)

A structured, end-to-end repository designed for mastering **Python for Data Science, Data Analysis, and Machine Learning**. This repository spans foundational Python programming, numeric computation with **NumPy**, tabular data manipulation with **Pandas**, web scraping, statistical visualization with **Matplotlib & Seaborn**, exploratory data analysis (EDA), and machine learning models with **Scikit-Learn**.

---

## 📌 Table of Contents

- [Overview](#-overview)
- [Repository Architecture](#-repository-architecture)
- [Curriculum & Notebooks Breakdown](#-curriculum--notebooks-breakdown)
  - [1. Core Python Fundamentals](#1-core-python-fundamentals)
  - [2. Numerical Computing with NumPy](#2-numerical-computing-with-numpy)
  - [3. Data Manipulation with Pandas](#3-data-manipulation-with-pandas)
  - [4. Web Scraping & HTML Tables](#4-web-scraping--html-tables)
  - [5. Statistical Data Visualization](#5-statistical-data-visualization)
  - [6. Machine Learning & Udemy Applied DS](#6-machine-learning--udemy-applied-ds)
  - [7. Hackathon Real-World Case Study](#7-hackathon-real-world-case-study)
- [Datasets Included](#-datasets-included)
- [Getting Started & Installation](#-getting-started--installation)
  - [Prerequisites](#prerequisites)
  - [Option A: Setup via `uv` (Recommended)](#option-a-setup-via-uv-recommended)
  - [Option B: Setup via `pip` & Virtual Environment](#option-b-setup-via-pip--virtual-environment)
  - [Option C: Setup via Conda](#option-c-setup-via-conda)
- [How to Run the Notebooks](#-how-to-run-the-notebooks)
- [Project Tech Stack](#-project-tech-stack)
- [Contributing](#-contributing)
- [Author & Acknowledgments](#-author--acknowledgments)

---

## 📖 Overview

The goal of this repository is to bridge the gap between initial Python programming concepts and applied Data Science workflows. Each notebook contains hands-on code cells, intermediate outputs, and real-world examples:

- **Core Python Essentials**: Syntax, dynamic typing, control flow, built-in data structures (lists, tuples, sets, dictionaries), and the standard `math` module.
- **NumPy Foundations**: High-performance multidimensional arrays, vectorized arithmetic, boolean masking, slicing, and matrix reshaping.
- **Data Wrangling with Pandas**: Loading various data sources (CSV, JSON, HTML), indexing with `.loc` / `.iloc`, aggregation, filtering, and cleaning.
- **Exploratory Data Analysis (EDA)**: Visualizing distributions, trends, and relationships using Seaborn joint plots, categorical plots, and facet grids.
- **Machine Learning Foundations**: Training regression and classification algorithms, evaluating metrics, and performing unsupervised K-Means clustering.

---

## 📂 Repository Architecture

```text
python_for_ds/
├── src/
│   └── python_for_ds/
│       └── __init__.py               # Python package entrypoint
│
├── lesson 1.ipynb                    # Variables, types, boolean logic, strings & control flow
├── lesson 4.ipynb                    # Comparison operators, identity, and Python math library
├── lesson 6.ipynb                    # Python Lists: operations, indexing, slicing & methods
├── lesson 7.ipynb                    # Sets, Dictionaries, and Tuples deep dive
├── numpy.ipynb                       # NumPy arrays, multidimensional slicing, vectorized ops
├── pandas.ipynb                      # Pandas Series/DataFrames, .loc/.iloc selection, filtering
├── pandas2.ipynb                     # In-memory CSV parsing, JSON serialization/deserialization
├── Py_html.ipynb                     # HTML table extraction via Pandas and web scraping
├── seaborn.ipynb                     # Statistical visualization with Seaborn (categorical/relational)
├── data science_udemy.ipynb          # End-to-end DS workflow: EDA, Regression & K-Means clustering
├── hackethon.ipynb                   # Real-world crash severity dataset exploratory analysis
│
├── flights.csv                       # Historical monthly international airline passengers
├── hack.csv                          # Vehicle crash severity and road safety dataset
├── mercedesbenz.csv                  # Kaggle Mercedes-Benz manufacturing feature dataset
├── demo.html                         # Exported HTML table from Wikipedia extraction
│
├── pyproject.toml                    # Modern PEP 621 packaging and dependency manifest
├── requirements.txt                  # Standard pip dependencies specification
├── .python-version                   # Default Python runtime pin (3.13)
├── .gitignore                        # Git ignore rules (clean checkpoints & virtualenvs)
└── README.md                         # Comprehensive documentation
```

---

## 🔬 Curriculum & Notebooks Breakdown

### 1. Core Python Fundamentals

| Notebook | Focus Areas | Key Concepts & Functions |
| :--- | :--- | :--- |
| **`lesson 1.ipynb`** | Python Basics & Control Flow | Data types (`int`, `float`, `complex`), type casting, dynamic typing, string concatenation & `.format()` string interpolation, user input with `input()`, boolean operations (`and`, `or`), conditional statements (`if-elif-else`), and `while` loop control with `break`. |
| **`lesson 4.ipynb`** | Operators & `math` Module | Boolean truth evaluations, comparison operators (`==`, `!=`, `<`, `>`), identity checks (`id()`), and standard `math` functions: `math.ceil()`, `math.floor()`, `math.exp()`, `math.fabs()`, `math.log()`, `math.log10()`, `math.pow()`, `math.sqrt()`, `math.cos()`, `max()`, `min()`. |
| **`lesson 6.ipynb`** | Lists & Sequence Operations | List construction, indexing and multi-level slicing, element iteration (`for` loops), in-place mutation methods (`append()`, `insert()`, `pop()`), nested lists, sequence replication (`lst * 3`), and aggregate functions (`sum()`, `len()`). |
| **`lesson 7.ipynb`** | Sets, Dictionaries & Tuples | **Sets**: Uniqueness, mutability, `.add()`. <br>**Dictionaries**: Key-value mapping, `.items()`, `.values()`, `.keys()`, dynamic key assignment. <br>**Tuples**: Immutability, `.count()`, `.index()`, and type casting between tuples and lists. |

### 2. Numerical Computing with NumPy

- **Notebook**: [`numpy.ipynb`](./numpy.ipynb)
- **Highlights**:
  - Converting Python lists into 1D and 2D `np.ndarray` structures.
  - Multi-axis slicing: step indexing (`arr[::2]`), array reversal (`arr[::-1]`), sub-matrix extraction (`arr1[1:, 1:3]`).
  - Shape manipulation: `.reshape()`, shape inspection via `.shape`.
  - Array generation routines: `np.arange()`, `np.ones()`, `np.zeros()`, `np.random.randint()`.
  - Vectorized operations: element-wise arithmetic, scalar broadcasting, and boolean mask filtering (`arr[arr < 2]`).

### 3. Data Manipulation with Pandas

- **Notebooks**: [`pandas.ipynb`](./pandas.ipynb) & [`pandas2.ipynb`](./pandas2.ipynb)
- **Highlights**:
  - **DataFrame & Series Core**: Generating DataFrames from matrix data with custom index and column labels.
  - **Data Inspection**: `.head()`, `.tail()`, `.info()`, `.describe()`, and `.isnull().sum()`.
  - **Selection & Slicing**: Label-based `.loc[]` vs integer-based `.iloc[]` row/column filtering.
  - **String Streams & IO**: Using `io.StringIO` to simulate streaming CSV files without disk overhead.
  - **Targeted Loading**: Using `usecols` with `pd.read_csv()` to optimize memory consumption when loading large datasets like `mercedesbenz.csv`.
  - **JSON Transformations**: Exporting and importing JSON across structural orientations (`orient='index'`, `'columns'`, `'records'`, `'split'`).

### 4. Web Scraping & HTML Tables

- **Notebook**: [`Py_html.ipynb`](./Py_html.ipynb)
- **Highlights**:
  - Automated HTML scraping with `pd.read_html()` using underlying parsers (`lxml`, `html5lib`, `BeautifulSoup`).
  - Scraping live Wikipedia data: Mobile Country Codes (MCC).
  - Filtering target tables directly at fetch time using regex/string patterns with the `match=` parameter.
  - Exporting parsed DataFrames back into standalone HTML tables (`demo.html`) via `df.to_html()`.

### 5. Statistical Data Visualization

- **Notebook**: [`seaborn.ipynb`](./seaborn.ipynb)
- **Highlights**:
  - Statistical plotting using **Seaborn** and **Matplotlib**.
  - Visualizing monthly passenger travel trends across years using the `flights.csv` dataset.
  - Utilizing categorical distribution plots (`sns.catplot`, `sns.barplot`, etc.) to communicate distribution insights.

### 6. Machine Learning & Udemy Applied DS

- **Notebook**: [`data science_udemy.ipynb`](./data%20science_udemy.ipynb)
- **Highlights**:
  - **Exploratory Data Analysis (EDA)**:
    - Bivariate analysis of tipping habits on the `tips` dataset with `sns.jointplot(x='tip', y='total_bill')`.
    - Multi-variable conditioning via `sns.FacetGrid(..., col='sex', hue='smoker')` with mapped scatter plots.
  - **Supervised Learning**:
    - Splitting features and targets with `train_test_split`.
    - Fitting and comparing `LinearRegression` and `LogisticRegression` models.
    - Model evaluation using `sklearn.metrics`.
  - **Unsupervised Learning**:
    - Generating synthetic isotropic Gaussian blobs with `sklearn.datasets.make_blobs`.
    - Fitting a `KMeans(n_clusters=5)` clustering model to identify centroids and segment unlabeled observations.

### 7. Hackathon Real-World Case Study

- **Notebook**: [`hackethon.ipynb`](./hackethon.ipynb)
- **Highlights**:
  - Practical data exploration for a vehicle safety and crash severity dataset (`hack.csv`).
  - Feature inspection across 14 categorical and numerical columns.
  - Frequency distribution audits with `.value_counts()` and missing data diagnostics.

---

## 📊 Datasets Included

| File | Records | Features | Summary |
| :--- | :--- | :--- | :--- |
| **`flights.csv`** | 144 | 3 | Historical time-series tracking monthly international flight passengers from 1949 to 1960. |
| **`hack.csv`** | 300 | 14 | Real-world crash analytics data detailing vehicle speed, speed limits, alcohol consumption, road conditions, seatbelt usage, and crash severity. |
| **`mercedesbenz.csv`** | 4,209 | 378 | Kaggle automotive benchmark dataset containing anonymized categorical and binary variables used for testing car configuration times. |
| **`demo.html`** | — | — | Clean HTML output of parsed international mobile network codes generated from `Py_html.ipynb`. |

---

## ⚙️ Getting Started & Installation

### Prerequisites

- **Python**: Version 3.10 or higher (Python 3.13 tested)
- **Package Manager**: `uv`, `pip`, or `conda`
- **Git**: Installed and configured on your local machine

---

### Option A: Setup via `uv` (Recommended)

[`uv`](https://github.com/astral-sh/uv) is an extremely fast Python package and project manager.

1. **Clone the repository:**
   ```bash
   git clone https://github.com/shubh593/Python-For-Data-Science.git
   cd Python-For-Data-Science
   ```

2. **Sync the virtual environment and install all dependencies:**
   ```bash
   uv sync
   ```

3. **Activate the virtual environment:**
   - **Windows (PowerShell):**
     ```powershell
     .venv\Scripts\Activate.ps1
     ```
   - **Linux / macOS:**
     ```bash
     source .venv/bin/activate
     ```

---

### Option B: Setup via `pip` & Virtual Environment

1. **Clone the repository:**
   ```bash
   git clone https://github.com/shubh593/Python-For-Data-Science.git
   cd Python-For-Data-Science
   ```

2. **Create and activate a virtual environment:**
   - **Windows:**
     ```powershell
     python -m venv .venv
     .venv\Scripts\Activate.ps1
     ```
   - **Linux / macOS:**
     ```bash
     python3 -m venv .venv
     source .venv/bin/activate
     ```

3. **Install dependencies:**
   ```bash
   pip install --upgrade pip
   pip install -r requirements.txt
   ```

---

### Option C: Setup via Conda

```bash
git clone https://github.com/shubh593/Python-For-Data-Science.git
cd Python-For-Data-Science
conda create -n python_ds python=3.11 -y
conda activate python_ds
pip install -r requirements.txt
```

---

## 🚀 How to Run the Notebooks

Once your virtual environment is active, start Jupyter Lab or Jupyter Notebook:

```bash
# Launch Jupyter Notebook
jupyter notebook

# Or launch JupyterLab
jupyter lab
```

This will open the Jupyter web dashboard in your browser (`http://localhost:8888`). You can open any `.ipynb` notebook and execute the cells sequentially (`Shift + Enter`).

---

## 🛠️ Project Tech Stack

- **Language**: Python 3.13
- **Data Structures & Computation**: [NumPy](https://numpy.org/)
- **Data Manipulation & Analysis**: [Pandas](https://pandas.pydata.org/)
- **Data Visualization**: [Matplotlib](https://matplotlib.org/) & [Seaborn](https://seaborn.pydata.org/)
- **Machine Learning**: [Scikit-Learn](https://scikit-learn.org/)
- **Scientific Computing**: [SciPy](https://scipy.org/)
- **Web Parsing**: [lxml](https://lxml.de/), [html5lib](https://github.com/html5lib/html5lib-python), [BeautifulSoup4](https://www.crummy.com/software/BeautifulSoup/)
- **Interactive Environment**: [Jupyter Notebook / IPython](https://jupyter.org/)
- **Project & Dependency Management**: [uv](https://github.com/astral-sh/uv) / [pip](https://pip.pypa.io/)

---

## 🤝 Contributing

Contributions, feedback, and improvements are always welcome!

1. Fork the Project (`git checkout -b feature/AmazingFeature`)
2. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
3. Push to the Branch (`git push origin feature/AmazingFeature`)
4. Open a Pull Request

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

---

## 👤 Author

**Shubham Shinde**
- GitHub: [@shubh593](https://github.com/shubh593)
- Email: [sshinde5930@gmail.com](mailto:sshinde5930@gmail.com)

*If you find this repository helpful for your data science journey, consider giving it a ⭐ on GitHub!*

>>>>>>> master
