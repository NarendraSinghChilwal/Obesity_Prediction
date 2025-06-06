# README.md

# ObesityPrediction_Project

This notebook builds and evaluates machine learning models to predict obesity status based on various health and lifestyle features. It covers data loading, exploratory data analysis, preprocessing, model training (e.g., SVM and Random Forest), evaluation with multiple metrics, and visualization of results.

## Contents

- **notebooks/OBESITY.ipynb**  
  - Loads a CSV dataset containing health and lifestyle variables.  
  - Performs exploratory data analysis (distribution plots, correlation heatmaps).  
  - Encodes categorical variables with LabelEncoder and scales numerical features using StandardScaler.  
  - Splits data into training and test sets.  
  - Trains classifiers such as Support Vector Machine (SVM) and Random Forest.  
  - Evaluates model performance using accuracy, precision, recall, F1 score, and ROC AUC.  
  - Visualizes results (confusion matrix heatmap, ROC curve).

## Repository Structure

ObesityPrediction_Project/
├── README.md
├── requirements.txt
├── .gitignore
└── notebooks/
└── OBESITY.ipynb


- **README.md**: Project overview, setup instructions, and dependencies.  
- **requirements.txt**: List of Python packages needed to run the notebook without errors.  
- **.gitignore**: Specifies files and folders Git should ignore (cache files, checkpoints, raw data).  
- **notebooks/OBESITY.ipynb**: The Jupyter notebook containing all code cells, narrative, and outputs.

## Setup & Usage

1. **Clone or download the repository**  
   Obtain the project files by cloning the GitHub repository or downloading a ZIP archive. Navigate into the project folder.

2. **Create and activate a Python virtual environment**  
   It is recommended to create a virtual environment to isolate dependencies. After creating the environment, activate it so that installations do not affect the system Python.

3. **Install project dependencies**  
   A `requirements.txt` file is provided. Install all required packages by running a pip installation command that reads from this file. This ensures you have the correct versions of libraries such as NumPy, pandas, scikit-learn, Matplotlib, and Seaborn.

4. **Prepare your data**  
   - Create a `data/` folder at the root of the repository if it does not already exist.  
   - Place the CSV dataset (e.g., `obesity_data.csv`) into the `data/` folder.  
   - In the notebook, verify that the data-loading cell points to `data/obesity_data.csv` (or your actual filename), for example:  
     ```python
     import pandas as pd
     df = pd.read_csv("data/obesity_data.csv")
     ```

5. **Open and run the Jupyter notebook**  
   Launch Jupyter Notebook (or JupyterLab) from within the activated virtual environment. In the file browser, navigate to the `notebooks/` folder and open `OBESITY.ipynb`. Run each cell in order to reproduce the entire prediction pipeline. The notebook will display exploratory plots, preprocessing steps, model training logs, evaluation metrics, and visualizations.

## Dependencies

All required packages are listed in `requirements.txt`. At minimum, this project uses:

- numpy  
- pandas  
- scikit-learn  
- matplotlib  
- seaborn  

If any additional libraries are used (e.g., for advanced visualization), add them to `requirements.txt` before installation.

---

# .gitignore

Byte-compiled or optimized files
pycache/
*.pyc

Jupyter notebook checkpoints
.ipynb_checkpoints/

Ignore raw dataset files in data/ (don’t commit large CSVs)
data/*.csv

Local virtual environment folders
venv/
env/


---

# requirements.txt

numpy>=1.25.0
pandas>=2.1.0
scikit-learn>=1.2.0
matplotlib>=3.7.0
seaborn>=0.14.0
