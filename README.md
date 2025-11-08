**SHAP Misclassification Analysis**
One‑page repo for the course follow‑along. Contains the numbered notebooks (Cell_1 … Cell_8) used in the live session.

**Quick start (recommended)**
We recommend Python 3.13< for best compatibility with SHAP wheels. If Python 3.13 works on your machine, the venv instructions below will also work.

**macOS (venv)**
1. python3.13 -m venv shapenv
2. source shapenv/bin/activate
3. python -m pip install --upgrade pip setuptools wheel
4. pip install shap pandas scikit-learn joblib matplotlib jupyterlab ipykernel
5. python -m ipykernel install --user --name=shapenv --display-name "Python (shapenv)"

**Windows PowerShell (venv)**
1. python3.13 -m venv shapenv
2. shapenv\Scripts\Activate.ps1
3. python -m pip install --upgrade pip setuptools wheel
4. pip install shap pandas scikit-learn joblib matplotlib jupyterlab ipykernel
5. python -m ipykernel install --user --name=shapenv --display-name "Python (shapenv)"

Conda (cross-platform, easiest)
conda create -n shapenv python=3.11 -c conda-forge shap pandas scikit-learn matplotlib jupyterlab ipykernel
conda activate shapenv

If `pip install shap` fails:
python -m pip install --upgrade pip setuptools wheel
python -m pip install cython numpy scipy
pip install shap

If build errors reference compilers, install Xcode Command Line Tools (mac) or Visual C++ Build Tools (Windows). Prefer conda-forge for classrooms.
