#  Crime Data Analysis
![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-013243?logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-11557c)
![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-4c72b0)
![DataCamp](https://img.shields.io/badge/DataCamp-Project-03EF62?logo=datacamp&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-success)

A Python data analysis project exploring the `crimes.csv` dataset to uncover patterns in crime frequency by time of day, location, and victim age group.

> This project is part of the [DataCamp Data Scientist with Python](https://www.datacamp.com/tracks/data-scientist-with-python) career track.
---

## Project Overview

This project analyzes a crimes dataset to answer three key questions:

1. **Peak Crime Hour** — Which hour of the day sees the most criminal activity?
2. **Peak Night Crime Location** — Which area has the most crimes committed between 10pm and 3:59am?
3. **Victim Age Distribution** — How are crimes distributed across different victim age groups?

---

## 📁 Dataset

| File | Description |
|------|-------------|
| `crimes.csv` | Raw crime records including time, location, and victim demographics |

---

##  Getting Started

### Prerequisites

- Python 3.8+
- `crimes` virtual environment (see setup below)

### Setup

1. **Clone the repository**

   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name
   ```

2. **Activate the virtual environment**

   ```bash
   # macOS/Linux
   source crimes/bin/activate

   # Windows
   crimes\Scripts\activate
   ```

3. **Run the analysis**

   ```bash
   python analysis.py
   ```

---

## 📊 Key Outputs

### `peak_crime_hour` *(int)*
The hour (0–23) with the highest frequency of crimes.

```python
peak_crime_hour = 12  # example output
```

### `peak_night_crime_location` *(str)*
The area name with the most crimes committed between **10:00 PM and 3:59 AM**.

```python
peak_night_crime_location = "Central"  # example output
```

### `victim_ages` *(pandas.Series)*
A Series indexed by age group labels showing the count of crimes per group.

```python
victim_ages = pd.Series({
    "0-17":  ...,
    "18-25": ...,
    "26-34": ...,
    "35-44": ...,
    "45-54": ...,
    "55-64": ...,
    "65+":   ...
})
```

---

## 🗂️ Project Structure

```
├── crimes.csv              # Source dataset
├── Crime analysis.ipynb    # Main analysis script
├── crimes/                 # Virtual environment
└── README.md               # Project documentation
```

---

## Technologies Used

- [Python](https://www.python.org/)
- [pandas](https://pandas.pydata.org/) — data manipulation and analysis
- [NumPy](https://numpy.org/) — numerical operations
- [Matplotlib](https://matplotlib.org/) - making informative graphs
- [Seaborn](https://seaborn.pydata.org/) - making countplots

---

## License

This project is for educational purposes as part of the DataCamp curriculum.
