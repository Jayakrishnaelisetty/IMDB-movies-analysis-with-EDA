# IMDB-movies-analysis-with-EDA
Here's a professional and beginner-friendly **project description** for your IMDB EDA task. You can use this for your portfolio, GitHub README, or resume project list.

---


---
 📁 Objective:

The goal of this project is to perform a comprehensive exploratory data analysis (EDA) on the IMDB Movies dataset to extract insights, clean the data, visualize key patterns, and understand factors influencing a movie's rating, runtime, revenue, and popularity.

---

### 🔍 Dataset Description:

* The dataset contains metadata for thousands of movies including:

  * 🎞️ Title, Genre, Director, Cast, Release Date
  * 🕒 Runtime
  * 💰 Budget and Worldwide Gross
  * ⭐ Average IMDb Rating
  * 🎯 Metascore
  * 🌍 Country, Language, and more

---

### 🛠 Steps Performed:

#### 1. **Data Cleaning**

* Removed rows with minimal missing data (e.g., Writer, Country, Cast).
* Converted `Budget` and `Worldwide Gross` from string to numeric format (removed `$`, `,`, and "estimated").
* Converted `Runtime` from string format ("2 hours 30 minutes") to total minutes (integer).
* Converted `Release Date` to proper `datetime` format.
* Standardized column names and data types.

#### 2. **Outlier Detection and Removal**

* Used boxplots and scatter plots to visually detect outliers.
* Removed extreme values for:

  * Runtime (e.g., > 240 minutes)
  * Budget (e.g., > \$400 million)
  * Worldwide Gross (e.g., > \$2 billion)
* Automated outlier removal using predefined thresholds across all numeric columns.

#### 3. **Univariate Analysis**

* Plotted distributions for numeric features like `Runtime`, `Budget`, `Rating`, `Metascore`.
* Analyzed skewness and spread of individual features.

#### 4. **Bivariate Analysis**

* Correlation heatmap for numeric variables.
* Scatter plots to explore relationships:

  * Budget vs. Gross Revenue
  * Runtime vs. IMDb Rating
  * Metascore vs. IMDb Rating

#### 5. **Categorical Analysis**

* Identified top countries producing the most movies.
* Grouped data to analyze average ratings across countries and genres.

---

### 📈 Key Insights:

* Budget and Worldwide Gross are positively correlated.
* Longer runtimes tend to have slightly higher IMDb ratings (up to a limit).
* Metascore and IMDb rating are moderately correlated.
* USA is the dominant movie-producing country in the dataset.
* Most movies are within the 90–150 minute runtime range.

---

### 📊 Tools Used:

* **Python** (Pandas, NumPy)
* **Seaborn & Matplotlib** for data visualization
* **Jupyter Notebook** for interactive development

---


