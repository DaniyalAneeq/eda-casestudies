# Investigating Netflix Movies and Guest Stars in The Office

## Project Overview
This project explores Netflix movie data to investigate whether the average duration of movies has been declining over time. The analysis examines movie trends from 2011 to 2020 and explores potential factors contributing to changes in movie duration.

## Dataset
The project uses two CSV files located in the `datasets/` folder:

- **netflix_data.csv**: Contains comprehensive Netflix content data including:
  - Show ID, type (Movie/TV Show), title, director, cast
  - Country, date added, release year, duration
  - Description and genre information

- **color_data.csv**: Additional data for color-coding visualizations based on genre categories

## Analysis Performed

### 1. Initial Trend Analysis
- Created a DataFrame from aggregated movie duration data (2011-2020)
- Visualized the trend using line plots to identify declining movie durations

### 2. Comprehensive Data Exploration
- Loaded and cleaned the full Netflix dataset
- Filtered for movies only (excluding TV shows)
- Created scatter plots to visualize duration vs. release year

### 3. Genre-Based Investigation
- Identified short movies (under 60 minutes)
- Analyzed genre distribution of short-duration content
- Found that Children's movies, Documentaries, and Stand-Up specials significantly contribute to lower average durations

### 4. Visual Analysis with Color Coding
- Color-coded scatter plots by genre:
  - Red: Children's content
  - Blue: Documentaries
  - Green: Stand-Up comedy
  - Black: Other genres
- Applied custom styling using matplotlib themes

## Key Findings
- While there appears to be a downward trend in movie durations, the decline is largely influenced by non-traditional movie genres
- Children's movies, documentaries, and stand-up specials cluster in the shorter duration range
- Traditional feature films maintain relatively consistent durations
- The conclusion: We cannot definitively say that movies are getting shorter without accounting for genre differences

## Technologies Used
- **Python 3.x**
- **pandas**: Data manipulation and analysis
- **matplotlib**: Data visualization
- **Jupyter Notebook**: Interactive development environment

## How to Run
1. Ensure you have Python 3.x installed
2. Install required dependencies:
   ```bash
   pip install pandas matplotlib jupyter
   ```
3. Navigate to the project directory
4. Launch Jupyter Notebook:
   ```bash
   jupyter notebook solved_notebook.ipynb
   ```
5. Run all cells to reproduce the analysis

## Project Structure
```
investigating-netflix-movies-and-guest-stars-in-the-office/
├── datasets/
│   ├── netflix_data.csv
│   └── color_data.csv
├── solved_notebook.ipynb
└── README.md
```

## Learning Outcomes
- Data manipulation with pandas DataFrames
- Data cleaning and filtering techniques
- Creating effective data visualizations
- Drawing insights from exploratory data analysis
- Understanding the importance of considering confounding variables in data analysis
