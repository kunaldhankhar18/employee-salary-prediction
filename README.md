# employee-salary-predictionSalary Prediction

A simple machine learning project that predicts the placement package (LPA) of a student based on their CGPA using linear regression and its regularized variants.

Dataset

placement.csv contains 200 rows with two columns:

Column	Description
cgpa	Student's CGPA (input feature)
package	Placement package in LPA (target)
Notebook

SALARY PLACEMENT.ipynb walks through the following steps:

Load and inspect the dataset with pandas.
Visualize the relationship between CGPA and package using seaborn / matplotlib.
Split the data into training and test sets (test_size=0.2, random_state=42).
Train a baseline Linear Regression model and evaluate it.
Train Ridge regression with a high regularization strength.
Train Lasso regression across a range of alpha values to observe coefficient shrinkage.
Report evaluation metrics: MAE, MSE, RMSE, and R² score.
Results (Linear Regression baseline)

Coefficient (m): 0.5743
Intercept (b): -1.0270
MAE: 0.2315
MSE: 0.0842
RMSE: 0.2901
R²: 0.7731
Note: the notebook also contains an intentionally incorrect cell (sns.scatterplot(df['cgpa']df['package'])) that throws a SyntaxError. It is kept as-is to show a learning moment about Python syntax.
Project Structure

SALARY PREDICTION/
├── placement.csv              # Dataset
├── SALARY PLACEMENT.ipynb     # Jupyter notebook with the full workflow
├── README.md                  # You are here
└── requirements.txt           # Python dependencies
Requirements

Install the dependencies with:

pip install -r requirements.txt
Dependencies:

pandas
numpy
matplotlib
seaborn
scikit-learn
jupyter
How to Run

Clone the repository:

git clone <your-repo-url>
cd "SALARY PREDICTION"
(Optional) Create and activate a virtual environment:

python -m venv venv
source venv/bin/activate        # macOS / Linux
venv\Scripts\activate           # Windows
Install dependencies:

pip install -r requirements.txt
Launch Jupyter and open the notebook:

jupyter notebook "SALARY PLACEMENT.ipynb"
Run all cells in order to reproduce the results.

Tech Stack

Python 3.x
Jupyter Notebook
pandas, numpy — data handling
matplotlib, seaborn — visualization
scikit-learn — model training and evaluation (Linear Regression, Ridge, Lasso)
