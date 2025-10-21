# E-commerce Shopping Behavior Analysis

**Goal:** Practice Pandas data manipulation and Seaborn/Matplotlib visualization to understand customer habits.

## Setup & Installation
This project downloads its own data automatically using the `kagglehub` library. No API key setup is needed.

---

### Option 1: `conda` (Recommended)
1.  Clone this repository.
2.  Create and activate the conda environment:
    ```bash
    conda env create -f environment.yml
    conda activate ecommerce-env
    ```
3.  Launch Jupyter:
    ```bash
    jupyter lab
    ```
4.  Open `notebooks/analysis.ipynb` and **run the first few cells** to download the data automatically.

---

### Option 2: `venv` / `pip`
1.  Clone this repository.
2.  Create and activate a virtual environment:
    ```bash
    python -m venv venv
    source venv/bin/activate 
    # On Windows: .\venv\Scripts\activate
    ```
3.  Install the required libraries:
    ```bash
    pip install -r requirements.txt
    ```
4.  Launch Jupyter:
    ```bash
    jupyter lab
    ```
5.  Open `notebooks/analysis.ipynb` and **run the first few cells** to download the data automatically.

---

## Project Structure
* `/notebooks/analysis.ipynb`: The main notebook. **Run this to download data.**
* `/data/`: Stores the converted `.parquet` file (ignored by Git).
* `/figures/`: Contains exported charts and plots.
* `environment.yml`: Environment file for `conda`.
* `requirements.txt`: Environment file for `pip`.

## Project Status
- [x] Create data-downloading pipeline (`notebooks/analysis.ipynb`)
- [ ] Load and inspect data
- [ ] Clean and standardize column names
- [ ] Perform Exploratory Data Analysis (EDA)
- [ ] Document key findings
