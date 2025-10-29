# E-commerce Shopping Behavior Analysis

**Goal:** Practice Pandas data manipulation and Seaborn/Matplotlib visualization to understand customer habits.

## Data Source
* **Origin:** Kaggle
* **Dataset:** [Shopping Behavior Dataset](https://www.kaggle.com/datasets/ahmadrazakashif/shopping-behavior-dataset) by Ahmad Raza Kashif
* **Note:** For reviewer convenience, the raw `shopping_behavior_updated.csv` file used for this analysis is included in the `/data/` directory of this repository. The notebook loads this local file.

## Key Insights (Highlights)
* **Spending Consistency:** Purchase amounts per transaction are remarkably consistent (~$60 median) across different age groups, genders, product categories, and seasons.
* **Male Dominance:** Male customers represent the majority (~68%) of transactions across all product categories in this dataset.
* **Popular Categories:** Clothing and Accessories are the most frequently purchased item categories.
* **Data Quality:** The dataset was found to be clean with no missing values.
*(See the Jupyter Notebook for detailed analysis and visualizations).*

## Setup & Installation

1.  **Clone this repository.** The required CSV dataset is included in the `/data/` folder.

2.  **Set up your Environment (Choose One):**

    * **Option A: `conda` (Recommended)**
        ```bash
        # Create and activate the environment
        conda env create -f environment.yml
        conda activate ecommerce-env
        ```

    * **Option B: `venv` / `pip`**
        ```bash
        # Create and activate the environment
        python -m venv venv
        source venv/bin/activate  # On Windows: .\venv\Scripts\activate

        # Install dependencies
        pip install -r requirements.txt
        ```

3.  **Launch JupyterLab:**
    ```bash
    jupyter lab
    ```

4.  **Open the Notebook:** Navigate to the `/notebooks/` folder and open `analysis.ipynb`. You can now run the cells directly.

---

## Project Structure
* `/notebooks/analysis.ipynb`: The main analysis notebook containing detailed steps and conclusions.
* `/data/`: Contains the raw dataset (`.csv`) and processed (`.parquet`) files.
* `/figures/`: Contains exported charts and plots.
* `environment.yml`: Environment file for `conda` users.
* `requirements.txt`: Environment file for `pip` users.

## Project Status
- [x] Load and inspect data from local CSV
- [x] Clean and standardize column names
- [x] Perform Univariate Analysis (Numerical & Categorical)
- [x] Perform Bivariate Analysis (Key Relationships & Heatmap)
- [x] Add Detailed Summary and Conclusions (in Notebook)
