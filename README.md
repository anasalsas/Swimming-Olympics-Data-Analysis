# 🏊 Swimming Olympics Data Analysis

## Project Overview
This project analyzes Olympic swimming data by transforming **unstructured Wikipedia tables into a clean and structured dataset** using Python.

The goal was to simulate a real-world data scenario where raw data is messy, inconsistent, and requires **web scraping, data cleaning, and transformation** before analysis.

---

## Objectives
- Collect Olympic swimming data directly from the web (Wikipedia)
- Clean and standardize inconsistent table formats
- Extract structured information (athlete, country, time, records)
- Perform exploratory data analysis (EDA)
- Generate insights and visualizations

---

## Data Source
- Wikipedia:
  - Men's Olympic swimming medalists  
  - Women's Olympic swimming medalists  

Data was collected programmatically using web scraping techniques.

---

## Process

### 1. Data Collection (Web Scraping)
- Used `requests` to fetch HTML content
- Used `BeautifulSoup` and `pandas.read_html()` to extract tables
- Handled multiple pages (men/women datasets)

---

### 2. Data Cleaning & Transformation
- Removed irrelevant and inconsistent tables (blacklist approach)
- Standardized column formats across different tables
- Split merged fields (e.g., athlete + country)
- Extracted:
  - Athlete names
  - Countries
  - Times (converted to seconds)
  - Records (WR, OR, etc.)
- Cleaned text using `regex`
- Handled missing and inconsistent values

---

### 3. Data Structuring
- Created a unified dataset (`df_final`) for event-level results
- Created a separate dataset for all-time medal tables (`df_medals`)
- Extracted additional features:
  - Event type (distance & style)
  - Year from Olympic Games

---

### 4. Exploratory Data Analysis (EDA)
- Dataset structure and validation checks
- Missing values analysis
- Distribution of medals by country and gender
- Identification of inconsistencies in historical records

---

### 5. Visualization
- Interactive charts using Plotly:
  - Top countries by medal count
  - Medal distribution by gender
  - Country-level comparisons

---

## Key Insights
- The **USA dominates Olympic swimming medal counts** across both genders
- Data from Wikipedia contains **structural inconsistencies**, requiring strong cleaning logic
- Some historical records contain missing or inconsistent time data
- Event formats and naming conventions vary significantly across tables

---

## Skills Demonstrated
- Python (Pandas, NumPy)
- Web scraping (BeautifulSoup, requests)
- Data cleaning & transformation
- Regex and string parsing
- Handling messy real-world data
- Data modeling and structuring
- Data visualization (Plotly)
- Analytical thinking

---

## Project Management & Workflow

To simulate a real-world project environment, this analysis followed a structured workflow:

- **Planning & data flow design (Miro):**  
  Defined the data pipeline, from data collection (web scraping) to transformation and analysis.

- **Task management & backlog tracking (JIRA):**  
  Organized tasks such as data collection, cleaning, transformation, and analysis into a structured workflow.

These steps helped ensure a clear, organized, and scalable approach to the project.

See the `images/` folder for workflow and backlog examples.

---

## Future Improvements
- Improve country detection using external reference datasets
- Automate data validation rules
- Expand analysis to include performance trends over time
- Build an interactive dashboard (Power BI / Streamlit)

---

## Contact
If you’d like to connect or discuss this project:

🔗 LinkedIn: [Ana Salsas](https://www.linkedin.com/in/anasalsas/) 

---

## Notes
This project focuses on **learning and demonstrating data skills**, especially handling messy, real-world data scenarios.
