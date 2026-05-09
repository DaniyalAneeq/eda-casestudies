# The Android App Market on Google Play

## Project Overview
This project provides a comprehensive analysis of the Android app market by examining over 10,000 apps from Google Play Store. The analysis explores app categories, ratings, pricing strategies, and user sentiment to derive insights for app development and marketing strategies.

## Dataset
The project uses two CSV files located in the `datasets/` folder:

- **apps.csv**: Contains detailed information about 10,000+ Google Play Store apps
  - App name, category, rating, reviews count
  - Size, number of installs, type (Free/Paid)
  - Price, content rating, genres
  - Last update date, current version, Android version compatibility

- **user_reviews.csv**: Contains 100 reviews per app with sentiment analysis
  - App name and review text
  - Sentiment classification (Positive/Negative/Neutral)
  - Sentiment polarity and subjectivity scores

## Analysis Performed

### 1. Data Cleaning
- Removed duplicate entries
- Cleaned special characters from `Installs` and `Price` columns
- Converted data types for numerical analysis

### 2. Category Distribution
- Identified 33 unique app categories
- Analyzed market share across categories
- Found that Family and Game apps dominate the market

### 3. App Ratings Analysis
- Calculated average app rating: **4.17**
- Created histogram showing rating distribution
- Observed that most apps are highly rated (skewed left distribution)

### 4. Size and Price Analysis
- Examined relationship between app size and ratings
- Analyzed pricing strategies across categories
- Found that top-rated apps typically range from 2-20 MB
- Most apps are priced under $10

### 5. Category-Based Pricing
- Medical and Family apps are the most expensive categories
- Some medical apps priced up to $80
- Game apps are reasonably priced (under $20)
- Filtered out "junk" apps (priced over $100) for accurate analysis

### 6. Free vs. Paid Apps
- Compared installation numbers between free and paid apps
- Found that paid apps have relatively lower installs than free apps
- The difference is less stark than expected

### 7. Sentiment Analysis
- Analyzed user review sentiment for free vs. paid apps
- Free apps receive more harsh comments (more negative outliers)
- Paid apps show higher median sentiment polarity
- Suggests paid apps may have higher quality on average

## Key Findings
- **Family** and **Game** categories dominate the Google Play Store
- Average app rating is **4.17**, with most apps highly rated
- Optimal app size for high ratings: **2-20 MB**
- **Medical** and **Family** apps command premium pricing
- Free apps receive more negative reviews than paid apps
- Paid apps generally maintain higher quality standards

## Technologies Used
- **Python 3.x**
- **pandas**: Data manipulation and analysis
- **numpy**: Numerical operations
- **matplotlib**: Static visualizations
- **seaborn**: Statistical data visualization
- **plotly**: Interactive visualizations
- **Jupyter Notebook**: Interactive development environment

## How to Run
1. Ensure you have Python 3.x installed
2. Install required dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn plotly jupyter
   ```
3. Navigate to the project directory
4. Launch Jupyter Notebook:
   ```bash
   jupyter notebook solved_notebook.ipynb
   ```
5. Run all cells to reproduce the analysis

## Project Structure
```
the-android-app-market-on-google-play/
├── datasets/
│   ├── apps.csv
│   └── user_reviews.csv
├── solved_notebook.ipynb
└── README.md
```

## Business Insights
- **For Developers**: Focus on Family and Game categories for maximum market reach
- **Pricing Strategy**: Keep apps under $10 for better adoption; medical apps can command premium pricing
- **App Size**: Optimize app size to 2-20 MB for better ratings
- **Quality Matters**: Paid apps should maintain high quality to justify pricing
- **User Sentiment**: Monitor reviews closely; free apps face harsher criticism

## Learning Outcomes
- Advanced data cleaning techniques
- Exploratory data analysis (EDA) best practices
- Statistical visualization with seaborn and plotly
- Sentiment analysis interpretation
- Deriving business insights from data
- Understanding mobile app market dynamics
