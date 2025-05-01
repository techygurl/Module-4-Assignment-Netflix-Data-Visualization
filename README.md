# 📊 Netflix Genre Analysis

This project explores and visualizes the most common genres and rating distributions of content on Netflix using Python and R. It also demonstrates how to display images (e.g., generated plots) in R using the `png` and `grid` libraries.

---

## 📁 Dataset

The dataset was renamed to `Netflix_shows_movies.csv` after unzipping. It contains metadata about Netflix movies and shows, including:
- Title
- Type (Movie/TV Show)
- Listed genres
- Rating
- Country
- Date added
- Duration, etc.

---

## 🔍 Objectives

- Perform data preparation by unzipping the dataset and renaming it to "Netflix_shows_movies."

- Address missing values in the dataset through data cleaning.

- Conduct data exploration, including generating data descriptions and performing statistical analysis.

- Create visualizations to represent the most watched genres and the distribution of ratings using Python libraries (Seaborn, Pyplot, and Matplotlib).

- Integrate one of the charts or visualizations into R.

- Save your work as a zipped file or push it to your GitHub repository. Include a README file with comprehensive instructions on accessing and interpreting your Python and R code. 

---

## 📌 Python Code Highlights

### ➕ Data Cleaning
```python
## 📊 Python: Load and Clean the Dataset

The dataset is first loaded using `pandas`, and basic cleaning steps are applied — removing duplicates and dropping rows with missing values.

```python
import pandas as pd

# Load the Netflix dataset
df = pd.read_csv("Netflix_shows_movies.csv")

# Remove duplicate entries
df = df.drop_duplicates()

# Drop rows with missing values
df_cleaned = df.dropna()


Use <code>```r</code> for R code

# Read and display the saved PNG image
img <- readPNG("C:/Users/Varnosafety INT/Downloads/topgenres.png")
grid::grid.raster(img)
