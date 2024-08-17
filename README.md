### **Steps in the Notebook:**

1. **Library Imports**:  
   * Essential libraries for data manipulation and visualization were imported: `pandas`, `numpy`, `matplotlib`, `seaborn`, and `missingno`.  
2. **Loading the Dataset**:  
   * The dataset was loaded using `pd.read_csv("Customer-Churn.csv")`.  
3. **Initial Data Exploration**:  
   * The first few and last few rows of the dataset were viewed using `data.head()` and `data.tail()` respectively.  
   * The dataset’s summary statistics were examined with `data.describe().T`.  
   * The data types of each column were checked with `data.dtypes`.  
   * Missing values in the dataset were assessed using `data.isnull().sum()`.  
   * The overall information about the dataset was reviewed with `data.info()`.

### **Additional Steps in the Notebook:**

4. **Missing Data Visualization**:  
   * Visualized missing data using a heatmap (`sns.heatmap`) and a bar chart (`msno.bar`) to understand the distribution and amount of missing data.  
5. **Handling Missing Data**:  
   * Identified that the "TotalCharges" column had missing values.  
   * Filled missing values in the "TotalCharges" column using the median value of that column.  
6. **Dropping Irrelevant Columns**:  
   * The "customerID" column was identified as irrelevant for analysis and subsequently dropped.  
7. **Exploring Numerical Data**:  
   * A subset of the dataset containing only numerical columns was created.  
   * Conducted univariate analysis on the "SeniorCitizen" column using a histogram and a box plot.  
8. **Distribution Insights**:  
   * Observed that the dataset is heavily skewed towards non-senior citizens, which could affect the analysis and modeling due to the imbalance in the dataset.

### **Challenges Faced:**

* **Missing Data**: The presence of missing data, particularly in the "TotalCharges" column, required imputation strategies. The chosen approach was to fill these missing values with the median, which is a common method to mitigate the impact of outliers.  
* **Imbalanced Data**: The analysis noted a significant skew in the "SeniorCitizen" column, where the majority of the data points represent non-senior citizens. This imbalance is critical and suggests that any further analysis, especially modeling, will need to account for this to avoid biased results.

