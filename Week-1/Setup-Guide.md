# Python setup
Install Python 3.11 or 3.12 and Git, or use Google Colab (https://colab.research.google.com/) without local installation.

## Local setup
```bash
git clone https://github.com/vipul-LLM/WIDS-6.0-WEEK-1.git
cd WIDS-6.0-WEEK-1
python -m venv .venv
```
Activate on Windows PowerShell: `.venv\Scripts\Activate.ps1`. On macOS/Linux: `source .venv/bin/activate`. If PowerShell blocks activation, use the environment's Python executable directly rather than changing system policy.
```bash
python -m pip install -r requirements.txt
python -m jupyter notebook
```
Open Week-1/Starter-Notebook.ipynb. Download the CSV using the dataset guide and place it inside the Week-1 folder (or upload it into Colab). Run cells in order. If using Colab, open the notebook via GitHub or upload it, then install missing libraries if needed.

## Debugging
Check the Python interpreter, notebook working directory and package versions before reinstalling anything. Use the first meaningful traceback and inspect the shape and column names of your dataframe. Do not commit .venv or dataset.csv.
