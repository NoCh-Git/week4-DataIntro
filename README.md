# Session 4 — Intro to Data Course

This repository contains the materials for **Session 4** of *Intro to Data Course*.  
- Slides: see [`slides/`](./slides/) folder  
- Notebooks: see [`notebooks/`](./notebooks/) folder 
---

## 📑 Session Outline
### Preprocessing & Feature Engineering

This session prepares a messy survey dataset for later modeling work. 

1. Inspect data types, missing values, duplicates, category labels, and suspicious values.
2. Apply row-wise cleaning rules: remove duplicates, standardise labels, and flag impossible values.
3. Choose a target and remove identifiers and target-leakage features.
4. Split the data into training and test sets.
5. Fit missing-value handling, categorical encoding, and scaling on the training set only.
6. Extract useful date information and create simple features from existing columns.
7. Use a preprocessing pipeline to apply the same workflow consistently to both sets.

By the end of the session, you should be able to make a reliable documented preprocessing pipeline for your own dataset.

---
## 🚀 Environment Setup

Before starting, please **fork this repository** and create a fresh Python virtual environment.  
All required libraries are listed in `requirements.txt`.

> ⚠️ If you encounter errors during `pip install`, try removing the version pinning for the failing package(s) in `requirements.txt`.  
> On Apple M1/M2 systems you may also need to install additional system packages (the “M1 shizzle”).

---

### macOS / Linux (bash/zsh)

```bash
# Select Python version (if using pyenv)
pyenv local 3.11.3

# Create and activate virtual environment
python -m venv .venv
source .venv/bin/activate

# Upgrade pip and install dependencies
pip install --upgrade pip
pip install -r requirements.txt
```

### Windows (PowerShell)
```bash
# Select Python version (if using pyenv)
pyenv local 3.11.3

# Create and activate virtual environment
python -m venv .venv
.venv\Scripts\Activate.ps1

# Upgrade pip and install dependencies
python -m pip install --upgrade pip
pip install -r requirements.txt
```

### Windows (Git Bash)
```bash
# Select Python version (if using pyenv)
pyenv local 3.11.3

# Create and activate virtual environment
python -m venv .venv
source .venv/Scripts/activate

# Upgrade pip and install dependencies
python -m pip install --upgrade pip
pip install -r requirements.txt
```

You’re now ready to run the session notebooks!

Deactivate the environment when you’re done:
```bash
deactivate
```
