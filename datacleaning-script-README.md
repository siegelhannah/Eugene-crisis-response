# Data Analysis

This Jupyter notebook performs the final data analysis on the Eugene crisis response dataset, including statistical tests, modeling, and visualization of results.

## Prerequisites

* Python 3.6+
* Jupyter Notebook/Lab
* Required libraries:
  * pandas
  * numpy
  * matplotlib
  * seaborn
  * scikit-learn
  * statsmodels (for statistical testing)

## Setup Instructions

1. Ensure you have completed the previous steps:
  
  * Run `datacleaning-script.ipynb` first to generate `clean_data.csv`
  * Optionally, review `EDA-and-engineering.ipynb` for context
2. If you need the raw data for reference:
  
  * Navigate to the `project-data` folder
  * Extract the contents of `zipped-raw-data.zip` in the same directory
3. Install required dependencies:
  
      pip install pandas numpy matplotlib seaborn scikit-learn statsmodels
  

## Running the Notebook

1. Launch Jupyter Notebook/Lab:
  
      jupyter notebook
  
  or
  
      jupyter lab
  
2. Open `data-analysis.ipynb` from the Jupyter interface
  
3. Run all cells:
  
  * Use Cell → Run All or run each cell with Shift+Enter
  * Pay attention to markdown cells for explanation of analysis steps
  * Some analyses or model training may take time to complete

## Key Components

This notebook contains:

* Final data preparation for analysis
* Statistical hypothesis testing
* Generating statistical summaries
* Final visualizations and interpretations
* Conclusions and recommendations

## Output

The notebook generates:

* Final analysis results
* Visualizations for presentation
* Potential recommendations based on the data

## Important Notes

* This notebook represents the culmination of the analysis pipeline
* All findings should be interpreted within the context of the project goals
* Results may vary based on any parameters or configurations you adjust
* The notebook includes markdown cells documenting key findings and conclusions
