
# 📺 Netflix Dataset Preprocessing

This repository contains a Jupyter notebook that demonstrates the data preprocessing steps performed on the Netflix dataset (`netflix_titles.csv`). The dataset includes metadata about movies and TV shows available on Netflix.

## 📁 Dataset
The dataset used is `netflix_titles.csv`, which includes features such as title, director, cast, country, date added, release year, rating, duration, and description.

## 🔧 Data Preprocessing Steps

1. **Library Imports**
   - Utilized `pandas` for data manipulation and `datetime` for date parsing.

2. **Data Loading**
   - Loaded the Netflix dataset using `pd.read_csv()`.

3. **Handling Missing Values**
   - Checked for missing values across all columns.
   - Filled missing entries with `"Unknown"` where appropriate.

4. **Removing Duplicates**
   - Identified and removed duplicate rows from the dataset.

5. **String Cleaning and Standardization**
   - Removed leading/trailing whitespaces in string fields.
   - Standardized text in columns like `country`, `listed_in`, and `description` to title case.

6. **Date Formatting (`date_added`)**
   - Replaced `"Unknown"` with `NaN` to facilitate parsing.
   - Converted to datetime format and reformatted to `dd-mm-yyyy` string.
   - Refilled missing dates with `"Unknown"` after formatting.

7. **Duration Parsing**
   - Parsed `duration` column to extract numerical duration and its type (e.g., minutes, seasons).
   - Created two new columns: `duration_num` and `duration_type`.

8. **Exporting Processed Data**
   - Saved the cleaned dataset to `Netflix_processed.csv`.

## 📦 Output
- `Netflix_processed.csv` — the final cleaned and formatted dataset.

## 📘 Notebook File
- `Netflix_datapreprocessing.ipynb` — contains all the preprocessing code and inline outputs.



