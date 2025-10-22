# E-commerce Shopping Behavior Analysis

**Goal:** Practice Pandas data manipulation and Seaborn/Matplotlib visualization to understand customer habits.

## Setup & Installation

1.  **Download the Data:**
    * Go to the Kaggle dataset page: [Shopping Behavior Dataset](https://www.kaggle.com/datasets/ahmadrazakashif/shopping-behavior-dataset)
    * Download the `shopping_behavior_dataset.csv` file.
    * Place the downloaded `.csv` file into the `/data/` folder within this project directory.
    *(Note: The `/data/` folder is ignored by Git via `.gitignore`.)*

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

4.  **Open the Notebook:** Navigate to the `/notebooks/` folder and open `analysis.ipynb`. You can now run the cells to load the local data and perform the analysis.

---

## Project Structure
* `/notebooks/analysis.ipynb`: The main analysis notebook.
* `/data/`: Contains the manually downloaded raw data (`.csv`) (ignored by Git).
* `/figures/`: Will contain exported charts and plots.
* `environment.yml`: Environment file for `conda` users.
* `requirements.txt`: Environment file for `pip` users.

## Project Status
- [ ] Load and inspect data from local CSV
- [ ] Clean and standardize column names
- [ ] Perform Exploratory Data Analysis (EDA)
- [ ] Document key findings