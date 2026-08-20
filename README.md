# Superhero Data Analysis with Pandas

A completed pandas data-analysis lab using a modified SuperHeroDb dataset. The project demonstrates a full workflow for loading, cleaning, reshaping, joining, aggregating, and visualizing data to answer business questions.

## Business Questions

1. What is the distribution of superheroes by publisher?
2. What is the relationship between height and number of superpowers, and does this differ based on gender?
3. What are the five most common superpowers in Marvel Comics vs. DC Comics?
4. Exploratory question: which gender has the highest median number of superpowers?

## Data

The repository contains two source datasets:

- `heroes_information.csv` — one row per superhero, including attributes such as publisher, gender, height, and weight.
- `super_hero_powers.csv` — Boolean indicators describing which heroes possess each superpower.

Height is measured in centimeters and weight in pounds.

## Analysis Workflow

The notebook performs the following steps:

- load both CSV files with pandas
- inspect shape, data types, and missing values
- remove rows missing publisher information
- normalize inconsistent Marvel and DC publisher labels
- visualize superhero counts by publisher
- transpose the powers DataFrame so heroes become rows
- reset the index while preserving hero names
- merge hero attributes with superpower data
- calculate a total power count for each hero
- filter invalid negative height values
- visualize height versus power count by gender
- isolate Marvel Comics and DC Comics
- aggregate Boolean powers using `groupby()` and `sum()`
- transpose and reset the grouped power table
- identify and visualize each publisher's five most common powers
- perform an additional exploratory analysis using median power count by gender

## Technologies

- Python
- pandas
- NumPy
- Matplotlib
- Jupyter Notebook / Google Colab

## Running the Project

Open `DS_Course0_Week1_Module5_DataPy.ipynb` in Jupyter Notebook, JupyterLab, VS Code, or Google Colab and run the cells from top to bottom.

The CSV files must remain in the same directory as the notebook so the relative file paths resolve correctly.

## Key Takeaways

This project demonstrates why data cleaning is a necessary part of analysis. Missing publisher values, inconsistent text labels, and sentinel values such as negative heights must be handled before results can be trusted.

It also demonstrates common pandas operations used in real analytical work: `read_csv`, `dropna`, string normalization, `transpose`, `reset_index`, `merge`, Boolean aggregation, `groupby`, filtering, sorting, and visualization.

## Repository Structure

```text
DS_Course0_Week1_Module5_DataPy/
├── DS_Course0_Week1_Module5_DataPy.ipynb
├── heroes_information.csv
├── super_hero_powers.csv
├── question_3.png
└── README.md
```

## Author

Steven Rouse
