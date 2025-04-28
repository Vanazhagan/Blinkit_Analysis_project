# Blinkit Sales Data Analysis using Python

## Description

This project performs an exploratory data analysis (EDA) on Blinkit grocery sales data using Python. The goal is to understand sales patterns, identify key performance indicators (KPIs), and visualize trends within the dataset. The analysis covers aspects like sales distribution across different item types, fat content, outlet characteristics, and establishment years.

## Data Source

The analysis uses an Excel file named `BlinkIT Grocery Data.xlsx`.

**Note:** The notebook currently loads the data from a specific local path (`D:\DATA_ANALYST.tutorial\POWER_BI_PROJECT\2-Blinkit Sales_data_project_BI\BlinkIT Grocery Data.xlsx`). To run this notebook, you will need to:
1. Obtain the `BlinkIT Grocery Data.xlsx` file.
2. Place it in the same directory as the notebook or update the file path in the code cell where `pd.read_excel` is used.

## Tools and Libraries

The following Python libraries are used in this analysis:

*   **Pandas:** For data manipulation and analysis.
*   **NumPy:** For numerical operations.
*   **Matplotlib:** For creating static, interactive, and animated visualizations.
*   **Seaborn:** For making attractive and informative statistical graphics (used for the bar plot by location type).
*   **Jupyter Notebook:** As the environment for running the code and documenting the analysis.

## Analysis Overview

The notebook follows these main steps:

1.  **Import Libraries:** Loading necessary Python packages.
2.  **Load Data:** Reading the sales data from the Excel file into a Pandas DataFrame.
3.  **Initial Data Exploration:** Displaying the first and last few rows (`head()`, `tail()`), checking the dataset's dimensions (`shape`), viewing column names (`columns`), and data types (`dtypes`).
4.  **Data Cleaning:**
    *   Identifying inconsistencies in the `Item Fat Content` column (e.g., 'low fat', 'LF', 'reg').
    *   Standardizing the values in `Item Fat Content` to 'Low Fat' and 'Regular'.
    *   *(Note: The notebook identifies NaN values in `Item Weight` during exploration but doesn't explicitly handle them in the provided code.)*
5.  **KPI Calculation:** Computing key business metrics:
    *   Total Sales
    *   Average Sales per item record
    *   Total Number of Item Records (Sales count)
    *   Average Rating
6.  **Data Visualization:** Creating various plots to understand sales distribution:
    *   Pie chart showing Sales by Item Fat Content.
    *   Bar chart showing Total Sales by Item Type.
    *   Bar chart showing Total Sales by Outlet Location Type and Item Fat Content.
    *   Line plot showing Total Sales by Outlet Establishment Year.
    *   Pie chart showing Total Sales by Outlet Size.
    *   Bar chart showing Total Sales by Outlet Location Type.

## Key Visualizations

*   **Sales By Fat Content:** A pie chart illustrating the proportion of total sales attributed to 'Regular' vs. 'Low Fat' items.
*   **Sales By Item Type:** A bar chart ranking item types by their total sales contribution.
*   **Fat Content by Outlet Tier for Total Sales:** A grouped bar chart comparing regular vs. low-fat item sales across different outlet location tiers.
*   **Total Sales by Outlet Establishment Year:** A line plot showing how total sales vary based on the year the outlet was established.
*   **Sales by Outlet Size:** A pie chart showing the sales contribution of different outlet sizes (Small, Medium, High).
*   **Sales by Outlet Location:** A bar chart comparing total sales across different outlet location tiers (Tier 1, Tier 2, Tier 3).

## Getting Started / How to Run

To run this analysis yourself:

### Prerequisites

*   Python 3.x installed
*   Pip (Python package installer) or Conda

### Installation & Execution

1.  **Clone the repository (if applicable):**
    ```bash
    git clone <repository-url>
    cd <repository-directory>
    ```
2.  **Install required libraries:**
    ```bash
    pip install pandas numpy matplotlib seaborn openpyxl
    ```
    *(Note: `openpyxl` is needed by pandas to read `.xlsx` files)*
3.  **Place the Data:** Ensure the `BlinkIT Grocery Data.xlsx` file is in the same directory as the notebook, or update the path in the notebook accordingly.
4.  **Launch Jupyter:**
    ```bash
    jupyter notebook
    ```
    or
    ```bash
    jupyter lab
    ```
5.  **Open and Run:** Open the `Blinkit_Analysis-Python.ipynb` file and run the cells sequentially.

---

Feel free to suggest improvements or add further analysis!
