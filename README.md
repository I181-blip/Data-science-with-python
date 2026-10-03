# Data-science-with-python
# Data Science with Python

My complete Data Analysis & Data Wrangling work for Data Clinic.

## Folder Structure
- `01_basics` - Python basics
- `02_data_analysis` - All notebooks and datasets
    - `data_wrangling.ipynb` - Cleaning missing values
    - `plot.ipynb` - All visualizations
    - `pandas_day5.ipynb` - Groupby analysis
    - `kashti.csv / kashti.xlsx` - Titanic dataset
    - `phool.xlsx` - Iris dataset

## Dataset 1: Titanic (Kashti)
**Source:** `sns.load_dataset('titanic')`

**Cleaning Done:**
- Found missing values: 177 in Age, 2 in Embarked
- Filled Age with median, Embarked with mode
- Fixed `Unnamed: 0` issue by using `index=False` while saving

**Key Findings:**
1. Only 38% Survived, 62% Died
2. Gender: Female survival 74% vs Male 19% - `countplot(hue="sex")`
3. Class: 1st class survived most, 3rd class died most - `countplot(hue="pclass")`
4. Age: Young males died most - `boxplot` and `violinplot(split=True)`

## Dataset 2: Iris (Phool)
- `pairplot(hue="species")`
- Setosa = smallest petals, Virginica = largest

## Libraries Used
pandas, seaborn, matplotlib, numpy

## How to Run
pip install pandas seaborn matplotlib
jupyter notebook

Author: Data Clinic Student
