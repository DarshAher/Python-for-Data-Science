# Python for Data Science

**Python for Data Science** is a comprehensive GitHub repository that serves as a learning resource and reference for anyone interested in data science with Python. It includes a collection of well-documented Jupyter notebooks, high-quality cheat sheets, sample datasets, and a detailed README to help users get started. Whether you’re a beginner learning the basics or a professional in need of a quick refresher, this repository provides clear examples and concise reference material in an easy-to-navigate structure.

## Topics Covered

* **Python Basics:** Core language features (data types, variables, operators), control flow (conditionals, loops), defining and using functions, and examples of basic coding patterns.
* **NumPy:** Creating and manipulating arrays, array indexing and slicing, element-wise operations, broadcasting rules, and using NumPy for numerical computations.
* **Pandas:** Working with DataFrames and Series, reading and writing data (CSV, JSON, Excel), data exploration and cleaning (handling missing values, removing duplicates), using `groupby` for aggregation, merging/joining datasets, date/time handling, and other essential data manipulation techniques.
* **Data Visualization:** Plotting with Matplotlib and Seaborn – creating line plots, bar charts, histograms, scatter plots, and more. Customizing plot aesthetics (titles, labels, legends) and using Seaborn for statistical visualizations and styling.
* **File I/O Operations:** Reading from and writing to various file formats using Python and pandas – including CSV files, JSON data, and Excel spreadsheets. Illustrative examples show how to use pandas I/O functions (like `read_csv`, `read_excel`, `to_csv`, etc.) to load and save data.
* **Data Preprocessing:** Techniques for preparing data for analysis – identifying and handling null or missing values, filling or dropping those entries, detecting and removing duplicate records, transforming text (string operations) and categorical data, and parsing dates and times into datetime objects for time-series analysis.

## Repository Structure

For convenience, the repository is organized into folders separating notebooks, cheat sheets, and datasets. All files are arranged for easy access and zip download. Below is an overview of the repository structure:

```plaintext
Python-for-Data-Science/
├── notebooks/
│   ├── 1_Python_Basics.ipynb          # Python language basics and examples
│   ├── 2_NumPy_Basics.ipynb           # Introduction to NumPy arrays
│   ├── 3_Pandas_Fundamentals.ipynb    # Data analysis with pandas
│   ├── 4_Data_Visualization.ipynb     # Matplotlib & Seaborn examples
│   ├── 5_File_Operations.ipynb        # Reading/Writing files with Python/pandas
│   └── 6_Data_Preprocessing.ipynb     # Data cleaning and preprocessing
├── cheat_sheets/
│   ├── Python_for_Data_Science_Cheat_Sheet.pdf
│   ├── NumPy_Cheat_Sheet.pdf
│   ├── Pandas_Cheat_Sheet.pdf
│   ├── Matplotlib_Cheat_Sheet.pdf
│   └── Seaborn_Cheat_Sheet.pdf
├── datasets/
│   ├── titanic.csv    # Titanic passenger data
│   ├── iris.csv       # Iris flowers data
│   └── air_quality.csv# Air quality sensor data
├── README.md          # Documentation and overview (this file)
└── LICENSE            # License information (MIT)
```

## Jupyter Notebooks

The `notebooks/` directory contains interactive Jupyter notebooks (`.ipynb` files) with step-by-step code examples, explanations, and comments. Each notebook focuses on a specific topic and demonstrates concepts through Python code and output. The notebooks are organized in a logical progression (as numbered above):

* **1\_Python\_Basics.ipynb:** Covers the fundamentals of Python programming. This notebook introduces basic **data types** (integers, floats, strings, booleans, lists, dictionaries, etc.), **variables** and operators, and shows how to use **control flow** structures like `if/else` statements and `for/while` loops. It also demonstrates how to define and call **functions** in Python, with plenty of simple examples and in-line comments explaining each concept. By the end of this notebook, a learner will understand core Python syntax and be able to write simple programs and functions.

* **2\_NumPy\_Basics.ipynb:** Introduces NumPy, the fundamental package for scientific computing with Python. It explains how to create NumPy **arrays** (from Python lists or with functions like `np.array`, `np.arange`, `np.ones`), and how to examine an array’s shape and data type. The notebook covers **array indexing and slicing** (including multi-dimensional arrays), and illustrates NumPy’s ability to broadcast operations across arrays (performing element-wise arithmetic without explicit loops). We include examples of common numerical computations using NumPy (such as computing mean, sum, standard deviation, etc.) and demonstrate how operations on NumPy arrays are much faster and more convenient than pure Python loops for large data.

* **3\_Pandas\_Fundamentals.ipynb:** A comprehensive tutorial on data manipulation with the pandas library. This notebook starts with how to **read data** into pandas (using `pd.read_csv` to load datasets into DataFrame objects). It uses realistic example data (like the Titanic dataset) to show how to inspect DataFrame contents (using methods like `head`, `info`, `describe`). We then cover **data cleaning** tasks: handling **missing values** (e.g. using `dropna()` or `fillna()` to remove or fill nulls), removing or identifying **duplicate** rows, and performing **string operations** on text columns (using `str.lower`, `str.replace`, etc.). The notebook also explores **data analysis** operations: using pandas **groupby** to aggregate data by category, performing **joins/merges** between DataFrames, working with **datetime** values (e.g. parsing date strings into datetime objects and extracting components like year or month), and other common tasks in data wrangling. By working through this notebook, users will learn how the **fast, flexible, and expressive** data structures in pandas make real-world data analysis easier, covering everything needed to **kickstart data science work with pandas**.

* **4\_Data\_Visualization.ipynb:** Demonstrates how to create visualizations in Python using **Matplotlib** and **Seaborn**. This notebook includes examples of basic plots with Matplotlib (line plots, bar charts, histograms, scatter plots, etc.), showing how to configure titles, labels, and legends for clarity. It then introduces Seaborn, a popular high-level visualization library built on Matplotlib that makes it easy to produce attractive statistical graphics. We walk through examples such as plotting distributions (with histograms and KDEs), creating box plots and violin plots for statistical insights, and generating scatter plot grids and regression plots with Seaborn. The notebook emphasizes how to choose appropriate chart types for different data and how to style plots. By the end, users will know how to visualize data trends and patterns using Python’s two main plotting libraries. (For quick reference, see the Matplotlib and Seaborn cheat sheets included in this repo – Matplotlib basics are introduced with code samples, and Seaborn usage is guided through the five key steps to build a plot in that library.)

* **5\_File\_Operations.ipynb:** Focuses on reading from and writing to files in common formats, a key part of working with real data. This notebook shows how to use Python’s built-in functions and pandas to **read** data from **CSV files**, **Excel spreadsheets** (`.xlsx`), and **JSON** files, and how to **write or export** data to these formats. For example, it demonstrates `pandas.read_csv()` and `pandas.to_csv()` for CSV, `pandas.read_excel()` for Excel files, and `pandas.read_json()` for JSON data. It also touches on Python’s basic file handling (using `open()` for text or CSV files) for completeness. We include tips on file paths and working with directories. After going through this notebook, users will know how to load data from various sources into Python and save their processed data. *(Note: pandas supports many different file formats out of the box – CSV, Excel, SQL, JSON, Parquet, and more – each provided by a convenient `read_*` function.)*

* **6\_Data\_Preprocessing.ipynb:** Covers essential data preprocessing techniques to clean and prepare data before analysis or modeling. Using examples (like the Air Quality dataset and others), this notebook demonstrates how to **detect and handle missing data** (identifying NaNs or placeholder values and using strategies like dropping or imputing missing values), and how to **remove duplicates** to ensure dataset integrity. It also shows **data type conversions** (for example, converting strings to datetime objects or categorical types), **feature extraction** from dates (like extracting day of week from a timestamp), and **string manipulations** for cleaning text fields (trimming whitespace, standardizing text case, parsing structured information from strings, etc.). By applying these techniques, the notebook illustrates how to transform raw, messy data into a cleaned form ready for analysis. This notebook provides a practical guide to the first steps of data cleaning, which are crucial in any data science project.

Each notebook is written with **extensive comments** and markdown explanations, making it easy to follow the logic and understand the purpose of each code snippet. Users can run these notebooks interactively to see the output of each step. The notebooks not only teach the syntax but also include **explanations of why** each concept is important, helping learners build an intuition for data science programming.

## Cheat Sheets

In addition to the interactive notebooks, the repository offers a set of **research-based cheat sheets** in the `cheat_sheets/` folder. These are high-quality, single-page (PDF) references for quick lookup of syntax and best practices. Each cheat sheet distills key points from documentation and expert sources into a concise summary, making them valuable as study guides or on-the-job references. The following cheat sheets are included:

* **Python\_for\_Data\_Science\_Cheat\_Sheet.pdf:** A handy one-page reference to core Python concepts and syntax geared toward data science tasks. It covers the Python basics needed for data science (variables, data types, collections, loops, functions, and example usages of essential standard libraries) in a condensed format – essentially “the Python basics that you need to do data science”. This cheat sheet is great for beginners to quickly remind themselves of Python language fundamentals and for practitioners to recall core patterns at a glance.

* **NumPy\_Cheat\_Sheet.pdf:** A cheat sheet focusing on NumPy, summarizing how to create and manipulate arrays and perform numerical computations. It is a quick reference for NumPy beginners, highlighting array initialization (e.g. using `np.array`, `np.zeros`, `np.linspace`), reshaping and combining arrays, common array operations (like arithmetic, aggregation functions, sorting), and the rules of broadcasting. With example code and brief notes, this cheat sheet helps users write efficient NumPy code without having to dig through documentation.

* **Pandas\_Cheat\_Sheet.pdf:** This cheat sheet provides a concise guide to the pandas data analysis library. It walks through the basics of using pandas for data wrangling – from different **data structures** (Series and DataFrame) to I/O routines (reading and writing data), data selection and subsetting, dropping or renaming columns, sorting data, getting summary information, applying functions, and aligning data. Essentially, the pandas cheat sheet **“guides you through the basics of the Pandas library, going from the data structures to I/O, selection, dropping indices or columns, sorting and ranking, retrieving basic information... to applying functions and data alignment”**. It’s a handy reference for anyone working with tabular data in Python.

* **Matplotlib\_Cheat\_Sheet.pdf:** A one-page **Matplotlib** reference that introduces the basics of plotting with Python. It outlines common plot types (line, bar, scatter, histogram, etc.) and the typical code to create them using `matplotlib.pyplot`. It also notes how to adjust plot elements like colors, markers, linestyles, titles, axes labels, and legends. This Matplotlib cheat sheet *“introduces you to the basics that you need to plot your data with Python and includes code samples”*, serving as a quick-start guide to producing charts and graphs for data visualization.

* **Seaborn\_Cheat\_Sheet.pdf:** A cheat sheet for the Seaborn library, which is built on Matplotlib for advanced statistical visualizations. It summarizes the high-level commands for creating attractive plots in Seaborn: for example, how to use **seaborn** to plot scatter matrices, line plots with confidence intervals, categorical plots (bar, box, violin plots), and heatmaps, all with a few function calls. It also covers the steps to get started with Seaborn (loading datasets, setting themes) and how Seaborn builds on Matplotlib. This cheat sheet *“guides you through the data visualization library that is based on Matplotlib”* with practical code examples and tips. It’s an excellent reference for quickly recalling Seaborn’s features and syntax.

All cheat sheets are provided in PDF format for easy viewing or printing. They condense information from official documentation and trusted tutorials into an easy-to-scan format, allowing users to quickly find the syntax or function they need without searching online. (For example, the pandas and NumPy cheat sheets in this repository were inspired by well-known references from DataCamp and the community, ensuring they cover the most important commands and patterns for data science work.)

## Sample Datasets

To make the examples in the notebooks concrete, the repository includes several **sample datasets** in the `datasets/` directory. These datasets are drawn from public sources (like Kaggle and the UCI Machine Learning Repository) and are classic examples used in data science education. Including them in the repository allows you to run the notebooks offline and experiment with the data directly. Below is a list of datasets provided, along with their sources:

| **Dataset**                                           | **Source (URL)**                                                                                               |
| ----------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- |
| **Titanic (passenger survival)** – `titanic.csv`      | [Kaggle – *Titanic: Machine Learning from Disaster*](https://www.kaggle.com/c/titanic)                         |
| **Iris (flower species)** – `iris.csv`                | [UCI Machine Learning Repository – *Iris* dataset](https://archive.ics.uci.edu/dataset/53/iris)                |
| **Air Quality (sensor readings)** – `air_quality.csv` | [UCI Machine Learning Repository – *Air Quality* dataset](https://archive.ics.uci.edu/dataset/360/air+quality) |

These datasets are well-known in the data science community:

* The **Titanic dataset** contains information on Titanic passengers (e.g. age, sex, passenger class, etc.) along with whether they survived the shipwreck. It is one of the most popular beginner datasets for practicing machine learning and data analysis. In this repository, we use Titanic data for examples of data cleaning (it has some missing values, like age) and for demonstrating pandas operations like grouping (e.g. comparing survival rates by gender or class). *(Source: Originally from a Kaggle competition, the data is included here in CSV form for convenience.)*

* The **Iris dataset** is a classic dataset in machine learning, first introduced by Ronald Fisher. It has 150 samples of iris flowers from three species (Setosa, Versicolor, Virginica) with four features (sepal length, sepal width, petal length, petal width). This small, clean dataset is often used to illustrate classification problems. We include it to demonstrate basic data analysis and visualization – for instance, plotting petal length vs petal width and seeing how the species differ. The Iris data is famously simple and well-structured: it contains 3 classes of 50 instances each (one for each iris species). *(Source: UCI Machine Learning Repository – the CSV is provided in the repo for easy access.)*

* The **Air Quality dataset** comes from the UCI repository and includes **9358 instances of hourly averaged responses from air quality sensor devices** in an Italian city, spanning one year. It’s a more complex dataset with time-series data and multiple sensor readings (CO, NOx, etc.), and it notably contains some missing values (which are tagged with a placeholder value of -200 in the dataset). We use this dataset in the preprocessing notebook to illustrate how to parse dates (it has separate date and time columns that can be combined) and how to handle missing data in a real-world scenario. *(Source: UCI ML Repository – included here under the filename `air_quality.csv`.)*

For each dataset, the README table above provides a link to the original source where you can find more detailed information. By bundling the data files in the repository, we ensure that the notebooks will run out-of-the-box. Users can also replace these with their own datasets to practice the demonstrated techniques on new data.

## Setup and Installation

To get started with this repository on your local machine, follow these steps:

1. **Clone or Download the Repository:** You can download the repository as a ZIP file and extract it, or use git to clone it:

   ```bash
   git clone https://github.com/yourusername/Python-for-Data-Science.git
   ```

   This will create a folder `Python-for-Data-Science/` with all the files.

2. **Install Python and Required Libraries:** Ensure you have **Python 3.x** installed on your system. It’s recommended to use a Python distribution like Anaconda for data science, which already includes most libraries. If you prefer to install manually, the key libraries used are **Jupyter Notebook**, **NumPy**, **pandas**, **Matplotlib**, and **Seaborn**. You can install these via pip:

   ```bash
   pip install numpy pandas matplotlib seaborn notebook
   ```

   This will install the core packages needed to run the notebooks. (Alternatively, you can use `conda` to create an environment: e.g., `conda install numpy pandas matplotlib seaborn jupyter`.)

3. **Launch Jupyter Notebook:** Navigate to the repository folder in your terminal:

   ```bash
   cd Python-for-Data-Science
   ```

   and launch the Jupyter Notebook server:

   ```bash
   jupyter notebook
   ```

   This will open the Jupyter interface in your web browser. From there, you can access the `notebooks/` directory and open any of the `.ipynb` files to interact with them.

4. **Run and Explore the Notebooks:** Once you have a notebook open, read the instructions and explanations provided. You can run each code cell sequentially (by pressing **Shift+Enter** in the cell). The notebooks are designed so that you can experiment – feel free to modify code or try new things. Each notebook is independent; you can start with the first one and work your way through, or jump directly to a topic of interest (for example, if you’re mainly interested in Pandas, open the pandas notebook). The sample datasets in the `datasets/` folder will be used by the notebooks (they assume the CSV files are in `../datasets/` relative to the notebook location), so keep the folder structure as is.

No additional setup is required beyond this. All data files are provided, and the notebooks contain all the code needed to produce the outputs and plots shown. If you encounter any issues (such as missing library dependencies), please refer to the requirements above and ensure all packages are installed.

## Repository Usage

* **Learning:** If you are using this repository to learn Python for data science, it’s recommended to go through the notebooks in order. The Python basics notebook will build your foundation, and later notebooks will build on those concepts. Make sure to read the markdown explanations in each notebook; they will guide you through the thought process and techniques. You can also use the cheat sheets to revise concepts quickly.

* **Reference:** For those already familiar with these topics, you can treat the notebooks and cheat sheets as reference material. The table of contents (Topics Covered) above can help you jump to whichever subject you need. For example, if you quickly need to remember how to do a groupby operation or the syntax for a Seaborn plot, you can consult the relevant notebook section or open the cheat sheet PDF for that topic.

* **Datasets:** The included datasets can be used to practice the demonstrated techniques. You might try extending the analysis – for instance, building a simple model on the Titanic data, or plotting additional relationships in the Iris data – to reinforce what you learned. Since these datasets are small, they are easy to work with interactively. Of course, you are welcome to bring in your own data (just place files in the `datasets/` folder or update the file paths in the code) to apply the code patterns to new scenarios.

* **Extensibility:** The repository is structured to be extendable. If you want to add your own notes or experiments, you can create new notebooks in the `notebooks/` directory. For example, you might add a `7_Scipy_ML.ipynb` for scikit-learn experiments or additional cheat sheets for other libraries – the README and structure can be updated accordingly.

## Author and License

**Author:** *Darshan S Aher* – This repository was created and is maintained by \Darshan S Aher. Feel free to reach out or contribute if you have suggestions or improvements.

**License:** This project is released under the MIT License, which means you are free to use, modify, and distribute the code and materials here. (See the `LICENSE` file for the full text of the license.) The included cheat sheets and documentation are also intended for open use. If reusing or redistributing, a mention of the source or a link back to this repository would be appreciated.  
