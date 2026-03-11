# netflix-data-analysis
Python-based exploratory data analysis of Netflix movies and TV shows dataset.

Netflix Data Analysis
Overview
This project performs exploratory data analysis (EDA) on the Netflix Titles dataset to uncover patterns in the platform's content library. The analysis focuses on understanding the distribution of movies and TV shows, the growth of Netflix content over time, and the geographic spread of content production.
The project demonstrates core data analysis skills including data cleaning, exploratory data analysis, and visualization using Python.

Dataset
Dataset: netflix_titles.csv
The dataset contains information about movies and TV shows available on Netflix.


Main Columns


Technologies Used
Python Pandas NumPy Matplotlib Seaborn Jupyter Notebook

Project Workflow
Data Loading
import pandas as pd
df = pd.read_csv("netflix_titles.csv")
Data Cleaning
df.fillna({
    "director": "Unknown",
    "cast": "Unknown",
    "country": "Unknown"
})
Exploratory Analysis
df["type"].value_counts()
Visualization
import seaborn as sns
import matplotlib.pyplot as plt

sns.countplot(data=df, x="type", color="#E50914")
plt.title("Distribution of Movies vs TV Shows")
plt.show()

Key Insights
Movies dominate the Netflix catalog compared to TV Shows.
The United States contributes a significant amount of Netflix content.
Netflix content growth accelerated significantly after 2015.

Project Structure
netflix-data-analysis/
│
├── netflix_analysis_.ipynb
├── netflix_titles.csv
└── README.md

How to Run
Clone repository:
git clone https://github.com/yourusername/netflix-data-analysis.git
Install dependencies:
pip install pandas numpy matplotlib seaborn
Run notebook:
jupyter notebook netflix_analysis_.ipynb

Author
Vivek
License
Educational and portfolio use.
