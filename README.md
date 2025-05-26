Task 1: Data Cleaning & Preprocessing

📄 Dataset

Used: `train_and_test2.csv` (custom Titanic-like dataset)

Tools Used

* Python
* Pandas, NumPy
* Matplotlib, Seaborn
* Scikit-learn

Steps Performed
1. Data Loading

* Loaded dataset using `pandas.read_csv()`
2. Column Cleanup

* Normalized column names using `.str.strip().str.lower()` to avoid KeyErrors
3. Data Exploration

* Used `.info()`, `.describe()` and `.isnull().sum()` to understand structure and missing data
4. Handling Missing Values

* Filled missing values in `age` using median
* Filled missing values in `embarked` using mode

5. Encoding Categorical Features

* Applied `pd.get_dummies()` to low-cardinality categorical columns
* Applied `LabelEncoder` to the `cabin` column

6. Feature Scaling

* Used `StandardScaler` from `sklearn` to normalize `age` and `fare`

7. Outlier Removal

* Detected and removed outliers using IQR method

8. Correlation Heatmap

* Plotted heatmap using `seaborn` to understand feature relationships

9. Data Export

* Saved the cleaned dataset as `cleaned_train_and_test2.csv`

Output

* Cleaned dataset ready for machine learning models
* Visual insights into data relationships
