# Python for Time Series Data Analysis

Time series analysis plays a vital role in forecasting and decision-making across finance, economics, and engineering. This repository introduces fundamental tools and coding practices for time series data analysis using Python. It is based on the Udemy course *“Python for Time Series Data Analysis”* by **Jose Portilla**, Head of Data Science at Pierian Training.  

These notes have been extended to include explanations. The repository will continue to evolve as more advanced chapters covering statistical and machine learning models.

---

### Programming Language

[Python](https://www.python.org/downloads/) / [Jupyter Notebook](https://jupyter.org/install)

### Data

Sample datasets used in these exercises are available in the `Data` folder of the repository. Each dataset corresponds to the examples provided in the notebooks.

---

### HTML Files

The `HTML Files` folder contains the **rendered Jupyter notebooks** for each chapter.  
These HTML files show both the **Python code and output (plots, tables, results)** without requiring a Jupyter environment.  
To view them:
1. Download the desired `.html` file from the folder.  
2. Open it locally in any modern web browser.  

This allows users to review the full notebook, including code, explanations, and figures, even without running Python.

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

## Chapter 4: Time Series with Pandas

This chapter focuses on **working with time-indexed data** using Pandas’ powerful date-time tools.  
It demonstrates how to parse, manipulate, resample, and visualize time series data effectively.

### **Objectives**
- Work with datetime indexes and perform time-based selection.  
- Parse and convert string timestamps.  
- Resample, shift, and aggregate data.  
- Visualize and interpret time-based trends.  
- Handle missing timestamps and time zone conversions.  

### **Topics Covered**
1. **Datetime Conversion and Indexing**  
   - Creating datetime indexes with `pd.date_range()` and `set_index()`.  
   - Parsing custom formats using `pd.to_datetime()`.  
2. **Selecting and Slicing by Date**  
   - Filtering data using `.loc[]` with partial string indexing.  
   - Extracting specific months, years, or ranges.  
3. **Resampling and Frequency Conversion**  
   - Downsampling (daily → monthly averages) and upsampling.  
   - Aggregating with functions like `mean`, `sum`, and `std`.  
4. **Rolling and Expanding Windows**  
   - Computing moving averages and cumulative statistics.  
   - Visualizing rolling and expanding metrics.  
5. **Shifting and Lagging Data**  
   - Comparing current vs. prior values using `.shift()`.  
6. **Date Arithmetic and Offsets**  
   - Adding or subtracting time periods (`'B'`, `'M'`, `'Q'`).  
   - Creating offset-based date ranges.  
7. **Handling Missing Dates and Reindexing**  
   - Filling gaps.  
8. **Visualizing Time Series Data**  
   - Plotting time-indexed Series and DataFrames using `plot()`.  
   - Adding titles, axis labels, gridlines, and custom ticks.  
   - Comparing raw vs. resampled or smoothed data visually.  

---


## Chapter 5: Time Series Analysis with Statsmodels

This chapter introduces **Statsmodels**, a Python library for building and interpreting statistical time series models.  
It focuses on trend–cycle decomposition, smoothing techniques, and exponential forecasting methods for understanding time-dependent data behavior.

### **Objectives**
- Understand the functionality of the `Statsmodels` library for time series analysis.  
- Perform **trend and cycle decomposition** using the Hodrick–Prescott filter.  
- Explore **Exponential Smoothing (ETS)** and **Holt-Winters** methods.  
- Apply and visualize **moving averages** and decomposed components.  
- Interpret the roles of trend, seasonality, and cyclical patterns in time series.

### **Topics Covered**
1. **Introduction to Statsmodels**  
   - Overview of the library and its role in econometrics and forecasting.  
   - Using built-in statistical tests and tools for time series analysis.  
2. **Hodrick–Prescott (HP) Filter**  
   - Separating trend and cyclical components of a time series.  
   - Understanding the smoothing parameter (`λ`) and its effect.  
   - Example: Decomposing the U.S. Real GDP data.  
3. **Time Series Components**  
   - Identifying trend, seasonality, and cyclical patterns.  
   - Visualization and interpretation of long-term movements.  
4. **ETS Decomposition**  
   - Additive and multiplicative decomposition of time series.  
   - Extracting trend, seasonal, and residual components.  
5. **Moving Average Techniques**  
   - Implementing simple and centered moving averages for smoothing.  
   - Visual comparison of raw vs. smoothed data.  
6. **Holt-Winters Exponential Smoothing**  
   - Modeling trend and seasonality in forecasting.  
   - Parameter tuning and forecast visualization.  

---


## Chapter 6: General Forecasting Models

This chapter introduces a comprehensive set of **statistical forecasting models** for analyzing and predicting time series data.  
It focuses on univariate and multivariate model structures, including ARIMA-based and vector autoregressive models, emphasizing model estimation, diagnostics, and forecasting accuracy evaluation.

### **Objectives**
- Understand the theory and implementation of **ARIMA-family models** for time series forecasting.  
- Learn to apply **seasonal** and **exogenous** model extensions such as SARIMA and ARIMAX.  
- Explore **multivariate models** including **VAR** and **VARMA** for systems of interrelated time series.  
- Perform model diagnostics, parameter selection, and forecast evaluation using statistical metrics.  
- Visualize fitted values, residuals, and forecast intervals for interpretability.

### **Topics Covered**
1. **Introduction to General Forecasting Frameworks**  
   - Overview of model-based forecasting in Python.  
   - Train–test splitting, model fitting, and forecast generation.  

2. **AR, MA, and ARIMA Models**  
   - Theoretical background of autoregressive and moving-average processes.  
   - Model identification and order selection using ACF and PACF.  
   - Estimation, diagnostics, and residual analysis.  

3. **SARIMA and ARIMAX Models**  
   - Seasonal ARIMA modeling for periodic time series.  
   - Incorporating external (exogenous) regressors with ARIMAX.  
   - Model selection using information criteria (AIC, BIC).  

4. **Vector Autoregressive (VAR) Models**  
   - Modeling interdependent time series using VAR.  
   - Lag selection and stationarity testing.  
   - Impulse response analysis and forecast visualization.  

5. **Vector Autoregressive Moving Average (VARMA) Models**  
   - Extending VAR models with moving-average components.  
   - Fitting and evaluating VARMA structures in Statsmodels.  
   - Comparing multivariate forecasts with univariate benchmarks.  

6. **Forecast Evaluation**  
   - Computing forecast errors such as MAE, RMSE, and MAPE.  
   - Comparing model performance over test periods.  
   - Visualizing actual vs. predicted series and confidence intervals.

---


## Future Chapters

The repository will continue to expand, focusing on advanced time series forecasting techniques, including:
 
- **Chapter 7:** Deep Learning Models for Time Series Forecasting
- **Chapter 8:** Focebook's Prophet Library

---

## References

Jose Portilla, *Python for Time Series Data Analysis*, Udemy.  

