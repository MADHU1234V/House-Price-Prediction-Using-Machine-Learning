# House Price Prediction Using Machine Learning

A regression project exploring how historical housing attributes can be used to estimate house prices. The repository separates exploratory data preparation from model training across two Jupyter Notebooks.

## Project objectives

- Clean and inspect housing data.
- Explore distributions, relationships, and potential outliers.
- Prepare features for regression.
- Train and evaluate regression models.
- Explain model performance using interpretable evaluation metrics.

## Technology stack

| Technology | Purpose |
|---|---|
| Python | Analysis and modeling |
| Jupyter Notebook | Interactive workflow |
| pandas / NumPy | Data manipulation |
| Matplotlib / Seaborn | Visualization and EDA |
| scikit-learn | Preprocessing, regression, and evaluation |

## Repository structure

```text
.
├── HousePrice-1.ipynb   # Data cleaning and exploratory analysis
├── HousePrice-2.ipynb   # Model training, evaluation, and prediction
├── Requirements         # Dependency list (no .txt extension)
├── LICENSE
└── README.md
```

## Setup

```bash
python -m venv .venv
```

Activate the environment:

```powershell
# Windows PowerShell
.\.venv\Scripts\Activate.ps1
```

```bash
# macOS/Linux
source .venv/bin/activate
```

Install the dependencies and launch Jupyter:

```bash
python -m pip install --upgrade pip
pip install -r Requirements
jupyter notebook
```

Run `HousePrice-1.ipynb` first, then `HousePrice-2.ipynb`. Ensure any dataset files referenced by the notebooks are available at the expected paths.

## Workflow

1. **Data inspection:** check shape, types, missing values, and duplicates.
2. **Exploratory analysis:** inspect target distribution and feature relationships.
3. **Preprocessing:** encode categorical variables and handle missing values where needed.
4. **Model development:** establish a baseline and compare regression algorithms.
5. **Evaluation:** report MAE, RMSE, and R² on held-out data.
6. **Interpretation:** explain the strongest drivers and known weaknesses of the model.

## Evaluation

No verified metrics are asserted in this README. After rerunning the notebook, record the selected model, train/test methodology, MAE, RMSE, and R². Compare models on the same held-out split and avoid reporting training-set performance as generalization performance.

## Future improvements

- [ ] Rename `Requirements` to `requirements.txt`.
- [ ] Document the dataset source, target units, and license.
- [ ] Add a clear model comparison table and actual test metrics.
- [ ] Save the final preprocessing/model pipeline for repeatable inference.
- [ ] Add a small prediction example and notebook screenshots.
- [ ] Add a reproducible environment and basic automated checks.

## License

See the included `LICENSE` file for the code's reuse terms. Dataset terms may be separate.
