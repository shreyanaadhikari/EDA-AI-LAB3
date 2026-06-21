# EDA-AI-LAB3
We were given to perform EDA for a dataset in our AI Lab Task. This is my final LAB report for which I have performed EDA on a particular dataset.  

📊 Overview

Exploratory Data Analysis (EDA) performed on the IMDB Movie Dataset as part of Lab 3. The goal: understand the dataset's structure, assess data quality, and uncover patterns and relationships between movie attributes like rating, votes, revenue, and runtime — before any modeling is attempted.

📁 Dataset

IMDB_Movie_Data.csv — 1000 movies across 12 columns:

ColumnDescriptionRank, TitleMovie identifiersGenre, Director, ActorsCategorical attributesDescriptionText summaryYear, Runtime (Minutes)Release year & lengthRating, Votes, MetascoreAudience & critic scoresRevenue (Millions)Box office earnings

✅ Tasks Performed

 Displayed sample rows (df.head())
 Identified data types of each column (df.dtypes, df.info())
 Checked for missing values (df.isnull().sum())
 Checked for and removed duplicate rows (df.drop_duplicates())
 Histograms for numerical columns + bar chart for categorical (Genre)
 Scatter plots and a pair plot for relationships between numerical variables
 Correlation matrix heatmap

🔍 Key Insights

Rating is left-skewed — most movies cluster between 6.5–7.5, with very few poor ratings.
Revenue is right-skewed — most movies earn modestly, with a small number of blockbusters pulling a long tail.
Drama is the most common genre by a wide margin (~510 movies), followed by Action and Comedy.
Votes ↔ Revenue is the strongest correlation in the dataset (0.64) — more popular movies tend to earn more, though with significant spread.
Rating ↔ Metascore is also strongly correlated (0.63) — audience and critic opinions largely agree.
Revenue ↔ Metascore is the weakest link (0.14) — critical acclaim and box office performance are largely independent.
Missing data found only in Revenue (Millions) (~12.8%) and Metascore (~6.4%); no duplicate rows present.

👩‍💻 Author

Shreyana Adhikari
BSc. CSIT (4th Semester) · St. Xavier's College, Kathmandu
