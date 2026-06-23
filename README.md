# Effect of Resources on the Efficiency-Fairness Tradeoff for Allocation Problems - FAccT 2026

## Setup

### Prerequisites
- Python 3.12.8
- `uv` package manager ([installation guide](https://docs.astral.sh/uv/getting-started/installation/))

### Creating a Virtual Environment

To create a virtual environment using `uv`, run:

```bash
uv venv
```

This command will create a `.venv` directory in your project.

### Installing Dependencies

Activate the virtual environment and install dependencies from `requirements.txt`:

**On macOS/Linux:**
```bash
source .venv/bin/activate
uv pip install -r requirements.txt
```

**On Windows:**
```bash
.venv\Scripts\activate
uv pip install -r requirements.txt
```

### Running Jupyter Lab

After activating the virtual environment and installing dependencies, launch Jupyter Lab:

```bash
jupyter lab
```

This will start the Jupyter Lab server and automatically open it in your default web browser. You can then access the notebooks in the project:
- `budget-modelling.ipynb`
- `budget-modelling-robustness-check.ipynb`
- `stylized_curves.ipynb`

## Data Directory Structure

The `data/` folder contains experiment results and datasets from various fairness-aware machine learning baselines:

### `data/baselines/`
Contains predictions and scores from different fairness methods:

- **`krishnaswamy/`** - Results from Krishnaswamy et al.'s fairness method across 19 different runs (0-18)
- **`rezaei/`** - Scores from Rezaei et al.'s approach with equal opportunity fairness constraint (`eqopp_san_maj_0.5` parameter) across 19 runs
- **`zafar/`** - Results from Zafar et al.'s fairness method with different regularization parameters

### `data/schenk/`
Pre-processed datasets or baseline data from Schenk et al. across 19 experimental iterations

### `data/suppressed_santarian/`
Experimental results using the suppressed Santarian fairness approach across 19 runs

### `figs/`
Directory for storing generated figures and visualizations from the notebooks

## Project Overview

This project analyzes fairness in machine learning algorithms through budget-based modelling and robustness checks, comparing various fairness-aware learning methods and their effectiveness.

## Citation
```bibtex
@inproceedings{singh2026effect,
    author = {Singh, Shubham and and Kanich, Chris and Kash, Ian A.},
    title = {Effect of Resources on the Efficiency-Fairness Tradeoff for Allocation Problems},
    year = {2026},
    isbn = {979-8-4007-2596-8/2026/06},
    publisher = {Association for Computing Machinery},
    url = {https://doi.org/10.1145/3805689.3812245},
    doi = {10.1145/3805689.3812245},
    booktitle = {Proceedings of the 2026 ACM Conference on Fairness, Accountability, and Transparency},
    series = {FAccT '26}
}
```

DOI: https://doi.org/10.1145/3805689.3812245
