# Project - Data Transformation and Automation

## Description
This project involves transforming and enriching movie data for a client in the highly competitive movie streaming services market. The project includes web scraping, data transformation, integration, and automation to produce enriched datasets. The final deliverables include processed data files, a Jupyter Notebook, an Alteryx workflow, and a descriptive report.

---

## Key Tasks

### **Part A: Data Gathering, Transformation, and Enrichment**
1. **Data Gathering**:
   - Scrape IMDb data for the top 500 movies released between 2018 and 2020.
   - Extract the following details: `movie_id`, `rank`, `title`, `year`, `rating`, and `votes`.
   - Save the scraped data in a structured format as `IMDb_TopVoted_Group6.csv`.

2. **Data Enrichment**:
   - Import `Movies.csv` (provided by the client) and the scraped `IMDb_TopVoted_Group#.csv`.
   - Clean and transform the scraped data (`df2`) to ensure consistency.
   - Merge the client’s dataset (`df1`) with the transformed IMDb data.
   - Rearrange the fields in the following order:
     ```
     movie_id, rank, title, originalTitle, description, year, votes, rating, runtimeMinutes, ratingCategory, genres
     ```
   - Export the enriched dataset as `Project_3_Part_A_Group6.csv`.

---

### **Part B: Automate Data Transformation and Integration**
1. **Create Alteryx Workflow**:
   - Import `IMDb_TopVoted_Group#.csv` and `Movies.csv` into the workflow.
   - Perform necessary data cleaning and transformation.
   - Merge the datasets to create the enriched dataset.
   - Sort the enriched dataset by `rank` in ascending order and rearrange the fields as follows:
     ```
     movie_id, rank, title, originalTitle, description, year, votes, rating, runtimeMinutes, ratingCategory, genres
     ```
   - Split the `genres` column into `genre01`, `genre02`, and `genre03`. Drop the original `genres` column.

2. **Export Outputs**:
   - Save the enriched dataset as `Project_3_Part_B_Group6.csv`.

3. **Create Report**:
   - Include a brief description of:
     - Data used to enrich the client’s dataset.
     - Data cleaning and transformation steps implemented.
   - Provide a screenshot of the Alteryx workflow.
   - Save the report as `Project_3_Part_B_Group6.doc`.

---

## Technologies Used
- **Programming Language:** Python
- **Tools and Libraries:**
  - Pandas
  - Jupyter Notebook
- **Automation Tool:** Alteryx

---

## Outputs
### **Part A Deliverables**:
1. Annotated Jupyter Notebook in `.IPYNB` format.
2. Jupyter Notebook saved as `.HTML`.
3. Scraped IMDb data saved as `IMDb_TopVoted_Group6.csv`.
4. Enriched dataset saved as `Project_3_Part_A_Group6.csv`.

### **Part B Deliverables**:
1. Alteryx workflow saved as `Project_3_Part_B_Group6.yxmd`.
2. Enriched dataset saved as `Project_3_Part_B_Group6.csv`.
3. Word document report saved as `Project_3_Part_B_Group6.doc`.

---

## How to Run the Project

### **Part A: Using Jupyter Notebook**
1. Clone the repository:
   ```bash
   git clone https://github.com/VijayAtheli1709/Project---Data-Transformation-and-Automation.git

Install the required libraries:

Copy code:
pip install pandas jupyter
Open the Jupyter Notebook:

Copy code:
jupyter notebook Project_3_Part_A.ipynb

Follow the annotations in the notebook to replicate the data gathering and enrichment process.

### Part B: Using Alteryx
Open the provided Alteryx workflow file (Project_3_Part_B_Group#.yxmd).
Execute the workflow to automate the transformation and integration.
Export the enriched dataset as instructed.

### Project Highlights
Demonstrates advanced data scraping, transformation, and integration techniques.
Uses Python for detailed data profiling and cleansing.
Employs Alteryx to automate workflows for efficiency and scalability.
Provides comprehensive documentation and outputs for reproducibility.

### Repository Structure
Project_Data_Transformation/
├── Part_A/
│   ├── Project_3_Part_A.ipynb
│   ├── Project_3_Part_A_Group6.csv
│   ├── IMDb_TopVoted_Group#.csv
│   ├── Movies.csv
├── Part_B/
│   ├── Project_3_Part_B_Group6.yxmd
│   ├── Project_3_Part_B_Group6.csv
│   ├── Project_3_Part_B_Group6.doc
└── README.md

