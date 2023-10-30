# Cloud-Hosted Notebook Data Manipulation of Data Science Project
### IDS-706 Miniproject# 9 by Yuwen Cai

[![cicd](https://github.com/Candice1121/Yuwen-IDS706-miniproject9/actions/workflows/cicd.yml/badge.svg)](https://github.com/Candice1121/Yuwen-IDS706-miniproject9/actions/workflows/cicd.yml)

---
**Dataset Source**
https://raw.githubusercontent.com/mwaskom/seaborn-data/master/iris.csv

---

**Summary**

This project serves to set up a cloud-hosted Jupyter Notebook on Google Colab and perform data manipulation tasks on a sample dataset

---
**Project Structure**

- **`Jupyter Notebook(descriptive.ipynb)`**:
  - Contains cells that calculate descriptive features and simple histogram visualization of a given dataset using Pandas.
  - Validated using the nbval plugin for pytest.

- **`Python Script(script.py)`**:
  - Executes descriptive statistics and visualization in a Python file using Pandas.
  - validated through pytest.

- **`lib.py(lib.py)`**:
  - Main functions to work with datasets include reading the file, accessing its statistics, and visualizing its features.

- **`Makefile`**:
  - `Install`: Install dependencies via `pip install -r requirements.txt`
  - `Test`: Run all tests (test_*.py, *.ipynb)
  - `Format`: Format code with Python black
  - `Lint`: Lint code with Ruff

- **`test_lib.py(test_lib.py)`**:
  - Test cases for the lib.py script.

- **`test_script.py(test_script.py)`**:
  - Test cases for the script.py script.

---

**Getting Started**

This section is included in ```descriptive.ipynb```

### Pandas Descriptive Statistics
![](/output/description.png)

### Sepal Length(cm) Distribution
![](/output/visualization_hist.png)

### Pass test cases
![](/output/pytest.png)

---

**Run**

### Some Makefile Commands
```commandline
make install
make format
make lint
make test
make run
```


