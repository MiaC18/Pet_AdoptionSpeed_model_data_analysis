# Pets

A pet adoption data analysis and prediction project. Built on data from the Malaysian PetFinder platform, this project analyzes key factors influencing pet adoption speed and builds predictive models.

## Project Structure

```
pets/
├── data/
│   ├── raw/                  # Raw data
│   │   ├── train.csv         # Training dataset
│   │   ├── BreedLabels.csv   # Breed labels (240 dog breeds + ~67 cat breeds)
│   │   ├── ColorLabels.csv   # Color labels (7 colors)
│   │   └── state_labels.csv  # Malaysian state labels
│   └── processed/            # Processed data
├── notebook/                 # Jupyter Notebook analysis
├── src/                      # Source code
├── report/                   # Report output
├── main.py                   # Entry point
├── pyproject.toml            # Project dependency configuration
└── README.md
```

## Tech Stack

- **Python** >= 3.13
- **Data Processing**: Pandas, NumPy
- **Visualization**: Matplotlib, Seaborn
- **Machine Learning**: Scikit-learn
- **Interactive Analysis**: Jupyter Notebook
- **Package Manager**: uv

## Quick Start

### 1. Install uv (if not already installed)

```bash
pip install uv
```

### 2. Create virtual environment and install dependencies

```bash
uv sync
```

### 3. Launch Jupyter Notebook

```bash
uv run jupyter notebook
```

## Data Description

Data sourced from the PetFinder.my adoption platform, including the following key features:

| Feature | Description |
|---------|-------------|
| Breed | 240 dog breeds + mixed breed, ~67 cat breeds |
| Color | 7 coat colors |
| State | 16 Malaysian states / federal territories |
| Others | Age, size, health status, photo count, etc. |

## License

For learning and research purposes only.
