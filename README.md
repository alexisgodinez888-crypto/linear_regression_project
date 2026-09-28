📊 Linear Regression Project
A clean and interactive linear regression analysis built in Python using Jupyter notebooks.
This project includes dropdown selectors for choosing regression variables, automatic environment setup, and support for Excel and CSV datasets.

🚀 Features
-Interactive dropdown selectors for choosing X and Y columns
-Supports CSV and Excel (.xlsx) datasets
-Clean regression workflow using pandas, numpy, and scikit‑learn
-Visualizations with matplotlib and seaborn
-Fully reproducible environment using requirements.txt

1. Create and activate the virtual environment
Windows (PowerShell)

#code for windows
python -m venv venv
.\venv\Scripts\activate

#code for MacOS or linux
python3 -m venv venv
source venv/bin/activate

2. Install the required packages
#code
pip install -r requirements.txt

3. Open the project
VS Code
-Open the folder
-Open the notebook
-Select the venv Python interpreter
-Restart the kernel if needed

📘 How to Use the Notebook
This notebook guides you through running a complete linear regression analysis using an interactive workflow. Follow the steps below to use it effectively.

1. Load Your Dataset
Place your dataset (CSV or Excel) inside the data/ folder.
In the notebook, update the file path if needed:
file_path = "../data/your_file.xlsx"
data = pd.read_excel(file_path) or data = pd.read_csv(file_path) for CSV

2. Select Your Regression Columns (Interactive Dropdowns)
The notebook includes dropdown menus powered by ipywidgets so you can choose your X and Y variables without editing code.

You will see two dropdowns:

X column → independent variable

Y column → dependent variable

Just click each dropdown and select the columns you want to use.

After selecting, click Confirm Selection to display your choices.

3. Build Regression Variables
Once you confirm your selections, the notebook automatically creates:
X = data[[x_col]]
y = data[y_col]
This prepares your data for regression.

The notebook also includes validation to ensure:
-Columns exist
-Columns are numeric
-No missing values
-Columns have variance
If something is wrong, the notebook will tell you exactly what to fix.

4. Run the Regression
The notebook uses scikit‑learn to fit a linear regression model:
-Train the model
-Print coefficients
-Print intercept
-Show model performance
-Display predictions
Everything runs automatically once X and Y are selected.

5. View Visualizations
The notebook generates:
-Scatter plots
-Regression line plots
-Distribution plots

