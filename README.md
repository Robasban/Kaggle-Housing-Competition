# Kaggle Housing Competition

This repository contains a notebook and data for the Kaggle House Prices competition.

Contents:
- `int-adv-ml-xgboost-gridcv-pipeline-housing.ipynb` — main notebook
- `train.csv`, `test.csv` — data files (already in workspace)

Quick start

1. Create and activate a virtual environment (created here as `./.venv`):

```bash
python3 -m venv .venv
source .venv/bin/activate
```

2. Upgrade pip and install dependencies:

```bash
pip install --upgrade pip
pip install -r requirements.txt
```

3. Run the notebook (from activated venv):

```bash
jupyter lab
# or
jupyter notebook
```

Git & GitHub

This script will initialize a git repo and (optionally) create & push a GitHub repository if you have the GitHub CLI (`gh`) authenticated.

If `gh` isn't available, create a repo on GitHub and add the remote manually:

```bash
git remote add origin git@github.com:<your-username>/Kaggle-Housing-Competition.git
git push -u origin main
```

Notes

- A lightweight `requirements.txt` is included. Adjust versions if you need reproducibility.
- The notebook logs predictions to `submission.csv`; this file is explicitly ignored in `.gitignore`.
