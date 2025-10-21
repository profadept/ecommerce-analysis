# E-commerce Shopping Behavior Analysis

**Goal:** Practice Pandas data manipulation and Seaborn/Matplotlib visualization to understand customer habits.

## Setup & Installation
This project features a robust script that automatically downloads its own data. It first tries to use the Kaggle API for a local file copy; if that fails, it falls back to the simpler `kagglehub` library.

---

### **Part 1: Kaggle API Setup (Optional but Recommended)**
To see the raw `.csv` file in your `data/` folder, follow these one-time setup steps for your operating system.

#### For macOS & Linux Users
1.  Go to `kaggle.com/account` and click "Create New API Token" to download `kaggle.json`.
2.  Open your terminal and run the following commands:
    ```bash
    # Create the hidden config folder
    mkdir -p ~/.config/kaggle

    # Move the token file into that folder
    mv ~/Downloads/kaggle.json ~/.config/kaggle/

    # Set secure permissions (read/write for you only)
    chmod 600 ~/.config/kaggle/kaggle.json
    ```

#### For Windows Users
1.  Go to `kaggle.com/account` and click "Create New API Token" to download `kaggle.json`.
2.  Open File Explorer.
3.  Navigate to `C:\Users\<Your-Username>\`.
4.  Create a new folder named `.kaggle`.
5.  Move the `kaggle.json` file from your `Downloads` folder into the new `.kaggle` folder.
*(The `chmod` command is not necessary on Windows, as file permissions are handled differently.)*

---

### **Part 2: Environment Setup & Running the Analysis**
Choose the option that matches your environment manager.

#### Option A: `conda`
1.  Clone this repository.
2.  Create and activate the conda environment:
    ```bash
    conda env create -f environment.yml
    conda activate ecommerce-env
    ```
3.  Launch JupyterLab: `jupyter lab`
4.  Open `notebooks/analysis.ipynb` and run the cells.

#### Option B: `venv` / `pip`
1.  Clone this repository.
2.  Create and activate a virtual environment:
    ```bash
    python -m venv venv
    source venv/bin/activate
    # On Windows: .\venv\Scripts\activate
    ```
3.  Install the required libraries: `pip install -r requirements.txt`
4.  Launch JupyterLab: `jupyter lab`
5.  Open `notebooks/analysis.ipynb` and run the cells.

---

## Project Status
- [x] Create data-downloading pipeline
- [ ] Load and inspect data from Parquet file
- [ ] Clean and standardize column names
- [ ] Perform Exploratory Data Analysis (EDA)
- [ ] Document key findings
