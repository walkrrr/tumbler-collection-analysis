# Tumbler Collection Data Analysis

## Overview
This project explores a dataset of a personal tumbler collection using Python.  
The analysis focuses on identifying patterns in brands, bottle sizes, and limited-edition items through exploratory data analysis and visualization.

The goal of the project is to practice data analysis workflows including data loading, cleaning, visualization, and interpretation.

---

## Dataset
The dataset was created from a manually tracked collection of tumblers.

Columns included in the dataset:

- **brand** – brand of the tumbler
- **model** – product model or name
- **color** – tumbler color
- **size_oz** – bottle size in ounces
- **limited_edition** – indicates whether the tumbler is a limited edition item

---

## Tools and Libraries
The analysis was performed using:

- Python
- Pandas
- Seaborn
- Matplotlib
- Jupyter Notebook / Google Colab

---

## Analysis Questions
This project explores the following questions:

- Which brands appear most frequently in the collection?
- What bottle sizes are most common?
- How many tumblers are limited-edition items?
- How do bottle sizes vary by brand?

---

## Visualizations
The notebook includes several visualizations such as:

- Brand distribution
- Bottle size distribution
- Limited edition vs standard items
- Brand vs size comparisons

These visualizations help identify trends within the collection.

---

## Project Structure

import seaborn as sns
import matplotlib.pyplot as plt

color_palette = {
    "Black": "black",
    "Pink": "pink",
    "Blue": "skyblue",
    "Green": "green",
    "Purple": "purple",
    "White": "lightgray",
    "Red": "red",
    "Yellow": "gold"
}

sns.countplot(data=df, x="color", palette=color_palette)
plt.xticks(rotation=45)
plt.title("Distribution of Tumbler Colors")
plt.show()

color_palette = {
    "rose quartz": "#F7CAC9",
    "cream": "#FFFDD0",
    "sage": "#9CAF88",
    "navy": "#1F3A5F",
}

plt.savefig("brand_distribution.png", bbox_inches="tight")

