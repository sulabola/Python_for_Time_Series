# Python for Time Series Data Analysis

Time series analysis plays a vital role in forecasting and decision-making across finance, economics, and engineering. This repository introduces fundamental tools and coding practices for time series data analysis using Python. It is based on the Udemy course *“Python for Time Series Data Analysis”* by **Jose Portilla**, Head of Data Science at Pierian Training.  

These notes have been extended to include explanations. The repository will continue to evolve as more advanced chapters covering statistical and machine learning models.

---

### Programming Language

[Python](https://www.python.org/downloads/) / [Jupyter Notebook](https://jupyter.org/install)

### Data

Sample datasets used in these exercises are available in the `Data` folder of the repository. Each dataset corresponds to the examples provided.

---

## Chapter 1: NumPy — Foundations of Numerical Computing

The **NumPy** library provides the foundation for numerical and scientific computing in Python.  
This chapter focuses on building arrays, performing basic arithmetic, and understanding how NumPy handles data efficiently.

### **Objectives**
- Create, manipulate, and inspect NumPy arrays.
- Perform mathematical operations and broadcasting.
- Generate random numbers and handle runtime warnings.

### **Topics Covered**
1. **Creating Arrays**
   - Using `np.arange()`, `np.zeros()`, `np.ones()`, and `np.eye()` to create arrays.
2. **Array Operations**
   - Element-wise operations and scalar arithmetic.  
   - Division-by-zero behavior and handling warnings.
3. **Indexing and Slicing**
   - Accessing and modifying parts of arrays.
4. **Random Number Generation**
   - Sampling using `np.random.rand()` and understanding uniform random variables.
5. **Basic Mathematical Operations**
   - Applying mathematical expressions directly to arrays.
6. **NumPy Arrays – Part II**
   - Demonstrating identity matrices and array broadcasting.

---

## Chapter 2: Pandas — Data Manipulation and Analysis

The **Pandas** library builds upon NumPy and provides flexible tools for data manipulation and analysis.  
This chapter introduces Series and DataFrame objects, their relationships, and common operations such as filtering, joining, and reading data from various sources.

### **Objectives**
- Understand Pandas Series and DataFrame structures.
- Perform arithmetic and alignment operations across Series.
- Learn data input/output techniques with CSV, Excel, and HTML data.

### **Topics Covered**
1. **Pandas Series**
   - Creating Series objects.
   - Performing element-wise operations between Series.
   - Automatic alignment by index.
2. **DataFrames — Part One**
   - Creating DataFrames from dictionaries and Series.
   - Accessing columns and understanding indexes.
3. **Arithmetic Operations**
   - Operations across multiple Series and DataFrames with automatic alignment.
4. **Handling Missing Data**
   - Understanding `NaN` results when indexes do not match.
5. **Data Input and Output**
   - Reading tabular data from CSV and Excel files using `pd.read_csv()` and `pd.read_excel()`.
   - Using `pd.read_html()` to extract tables from web pages (requires `lxml`, `html5lib`, and `BeautifulSoup4`).
   - Writing data to files.
6. **Dropping Unwanted Columns**
   - Using `df.drop()` to remove unnecessary columns like `"Unnamed: 0"`.

---

## Chapter 3: Data Visualization with Pandas

This chapter explores how to create **data visualizations** directly with Pandas using its built-in plotting capabilities (powered by **Matplotlib**).  
It demonstrates how to visualize data trends, distributions, and comparisons efficiently to support exploratory data analysis (EDA).

### **Objectives**
- Understand how to generate plots directly from Series and DataFrames.  
- Learn different types of plots for numerical and categorical data.  
- Customize visual elements such as titles, labels, legends, and gridlines.  

### **Topics Covered**
1. **Line Plots**
   - Visualizing time series and sequential data using `DataFrame.plot()`.  
   - Overlaying multiple Series in one figure for comparison.  
2. **Bar and Horizontal Bar Charts**
   - Displaying and comparing categorical variables.  
   - Adjusting colors, figure sizes, and labels.  
3. **Histograms**
   - Exploring frequency distributions of numerical variables.  
   - Understanding data skewness and spread.  
4. **Boxplots**
   - Summarizing data variability and detecting outliers.  
5. **Area and Pie Charts**
   - Representing proportions and cumulative trends.  
6. **Scatter Plots**
   - Examining relationships between two quantitative variables with `kind='scatter'`.  
7. **Subplots and Styling**
   - Creating multiple plots in one figure.  
   - Customizing themes, titles, legends, and gridlines for better presentation.  


---

## Future Chapters

The repository will continue to expand, focusing on advanced time series forecasting techniques, including:

- **Chapter 4:** Time Series with Pandas  
- **Chapter 5:** Time Series Analysis with Statsmodels 
- **Chapter 6:** Generating Forecasting Models 
- **Chapter 7:** Deep Learning Models for Time Series Forecasting
- **Chapter 8:** Focebook's Prophet Library

---

## References

Jose Portilla, *Python for Time Series Data Analysis*, Udemy.  

