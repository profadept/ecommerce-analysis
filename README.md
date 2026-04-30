# E-commerce Shopping Behavior Analysis

An exploratory analysis of customer shopping behavior, answering three questions:

* Does gender or age group drive differences in purchase behavior?
* Which product categories dominate purchases, and does season or gender shift those preferences?
* Does the purchase amount vary meaningfully across customer segments?


## Key Findings

* **Demographics do not drive purchase behavior.** The purchases are spread across all age groups; the median purchase of both genders is 60.
  
* **Clothing and accessories dominate, regardless of season or gender.** Neither seasonality nor gender shifts category preference, indicating consistent demand across the customer base.
  
* **Customer segments do not differentiate spending.** Purchase amounts cluster around a median of $60 across categories and subscription status, reflecting a narrow product price range.


## Data Source
* **Origin:** Kaggle
* **Dataset:** [Shopping Behavior Dataset](https://www.kaggle.com/datasets/profadept/shopping-behaviour-dataset)

## Project Structure
```
.
├── data/                     # Raw and processed data files (gitignored)
├── figures/                  # Generated charts (gitignored)
├── notebooks                 
│   └── analysis.ipynb        # Main analysis notebook
├── pyproject.toml            # Project dependencies and metadata
├── README.md
├── scripts
│   └── download_data.py      # Kaggle dataset downloader
└── uv.lock                   # Locked dependency versions
```

## Setup

Requires [uv](https://docs.astral.sh/uv/). Clone the repo and sync dependencies:

```bash
git clone git@github.com:profadept/ecommerce-analysis.git
cd ecommerce-analysis
uv sync
```

## How to Run 

**Option 1 — Manual download**
Create a `data/` folder in the project root, download and unzip from the Kaggle 
link above, then place `shopping_behavior_updated.csv` inside it.

**Option 2 — Download script**
Place your Kaggle credentials at `~/.kaggle/kaggle.json`, then run:

```bash
uv run python scripts/download_data.py
```

Then launch the notebook:

```bash
uv run jupyter lab
```

## Tech Stack
- Python 3.14
- pandas, NumPy, seaborn, matplotlib
- Jupyter Lab
- uv for dependency management