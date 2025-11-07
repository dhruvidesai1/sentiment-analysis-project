-----

# PROJECT README: Employee Sentiment Analysis

-----

This repository contains the analysis for the Employee Sentiment Analysis project. The main goal was to use NLP and statistical modeling on an unlabeled email dataset (`test.csv`) to gauge organizational morale, track sentiment trends, and identify potential high-risk employees.

The analysis is fully contained within the **`Sentiment_Analysis.ipynb`** Jupyter Notebook.

Project Deliverables

This project successfully implemented all required analysis tasks:

| Feature | Description |
| :--- | :--- |
| **Sentiment Labeling** | Used the VADER lexicon to categorize every email as Positive, Negative, or Neutral. |
| **EDA** | Visualized monthly email volume and the overall distribution of sentiment. |
| **Monthly Scoring** | Calculated and plotted the average compound sentiment score over the project's timeline. |
| **Employee Ranking** | Ranked employees by email count, and identified those with the highest positive and negative contribution counts. |
| **Flight Risk** | Identified potential flight risks based on a heuristic combining high negative sentiment (Average Score \< -0.1) and sufficient activity (Count $\geq 5$). |
| **Linear Regression** | Developed a model using `sklearn` to quantify the long-term trend in monthly sentiment. |

-----


Repository Contents

| File/Folder | Purpose |
| :--- | :--- |
| **`Sentiment_Analysis.ipynb`** | The main notebook containing all Python code, execution, outputs, and model training. |
| **`test.csv`** | The raw, unlabeled input dataset used for the analysis. |
| **`visualization/`** | Folder containing all generated charts and plots (`.png` files). |

-----

## 4\. Execution and Setup

To reproduce these results, ensure you have the required libraries installed and run the notebook:

### Prerequisites

```bash
pip install pandas numpy matplotlib seaborn scikit-learn nltk
```

### Execution Steps

1.  Place **`test.csv`** in the project directory.
2.  Open **`Sentiment_Analysis.ipynb`**.
3.  Run all cells sequentially. The code will handle data cleaning, modeling, and output generation.
