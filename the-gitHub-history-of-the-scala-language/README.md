# The GitHub History of the Scala Language

## Project Overview
This project analyzes the real-world development history of Scala, a mature programming language with almost 30,000 commits spanning over ten years. By mining data from Git version control and GitHub, we explore contribution patterns, identify key contributors, and assess project health and activity.

## Dataset
The project uses three CSV files located in the `datasets/` folder:

- **pulls_2011-2013.csv**: Pull request data from late 2011 to end of 2013
  - Pull request ID (pid)
  - User/contributor name
  - Date of pull request

- **pulls_2014-2018.csv**: Pull request data from 2014 to 2018
  - Same structure as above
  - Covers more recent development period

- **pull_files.csv**: Files modified by each pull request
  - Pull request ID (pid)
  - File path that was modified

## Analysis Performed

### 1. Data Preparation
- Combined pull request data from two time periods (2011-2018)
- Converted date strings to DateTime objects with UTC timezone
- Merged pull request and file modification data

### 2. Project Activity Analysis
- Calculated monthly pull request counts over the project lifetime
- Visualized contribution trends using bar charts
- Assessed whether the project is actively maintained

### 3. Community Structure Analysis
- Analyzed distribution of contributions per user
- Created histogram showing number of pull requests per contributor
- Evaluated whether the project welcomes new contributors

### 4. Hot Spots Identification
- Identified files changed in the last 10 pull requests
- Found 55 unique files recently modified
- Focused on compiler, reflection, and testing components

### 5. Expert Identification
- Analyzed contribution history for specific files
- Identified top contributors to `Calculate.scala`:
  - **xeno-by**: 11 contributions
  - **retronym**: 5 contributions
  - **soc**: 4 contributions

### 6. Recent Activity Analysis
- Examined the last 10 pull requests for specific files
- Identified currently active contributors
- Found **retronym** as the most recent active contributor

### 7. Contributor Trend Analysis
- Compared contribution patterns of key developers over time
- Visualized yearly contribution counts for **xeno-by** and **soc**
- Analyzed file-specific expertise and recent involvement

## Key Findings
- Scala project shows consistent activity over the analyzed period
- The project has a healthy distribution of contributors
- Recent activity concentrated in compiler and reflection components
- **retronym** is the most recently active contributor to critical files
- **xeno-by** has the highest historical contribution count for specific components
- The project appears welcoming to new contributors based on contribution distribution

## Technologies Used
- **Python 3.x**
- **pandas**: Data manipulation and time series analysis
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
   jupyter notebook solved-notebook.ipynb
   ```
5. Run all cells to reproduce the analysis

## Project Structure
```
the-gitHub-history-of-the-scala-language/
├── datasets/
│   ├── pulls.csv
│   ├── pulls_2011-2013.csv
│   ├── pulls_2014-2018.csv
│   └── pull_files.csv
├── solved-notebook.ipynb
└── README.md
```

## Practical Applications
- **For Contributors**: Identify the right experts to contact for specific code areas
- **Project Health Assessment**: Evaluate whether an open-source project is actively maintained
- **Community Analysis**: Understand if a project welcomes new contributors
- **Code Navigation**: Find "hot spots" where active development is occurring
- **Expert Identification**: Locate knowledgeable developers for specific components

## Learning Outcomes
- Working with version control system data
- Time series analysis with pandas
- Grouping and aggregating data effectively
- Visualizing contribution patterns
- Understanding open-source project dynamics
- Data-driven decision making for open-source contributions
