# Eugene Crisis Response Data Analysis Project

This repository contains a data science analysis project focused on Eugene crisis response data. The project is organized into three Jupyter notebooks that should be run in sequence.

## Repository Contents

* `datacleaning-script.ipynb`: Initial data cleaning and preprocessing
* `EDA-and-engineering.ipynb`: Exploratory data analysis and feature engineering
* `data-analysis.ipynb`: Final data analysis and visualization
* `project-data/zipped-raw-data.zip`: Compressed raw datasets used by the notebooks

## Setup Instructions

1. Clone this repository to your local machine
2. Ensure you have Python 3.6+ and Jupyter Notebook/Lab installed
3. Install required dependencies:
  
      pip install pandas numpy matplotlib seaborn scikit-learn
  
4. Extract the raw datasets:
  * Navigate to the `project-data` folder
  * Extract the contents of `zipped-raw-data.zip` in the same directory

## Running the Notebooks

Follow these steps to run the complete analysis:

1. **First:** Run `datacleaning-script.ipynb`
  
  * This will process the raw data files and generate `clean_data.csv`
  * The clean data file will be saved in the project directory
2. **Second:** Run `EDA-and-engineering.ipynb`
  
  * This notebook uses the `clean_data.csv` file created in step 1
  * It performs exploratory analysis and feature engineering
3. **Third:** Run `data-analysis.ipynb`
  
  * This notebook uses the `clean_data.csv` file created in step 1
  * It performs the final analysis and generates visualizations

## Important Notes

* The notebooks must be run in the correct order as described above
* Each notebook has its own detailed README with specific instructions
* Ensure all data files are extracted before running any notebooks
