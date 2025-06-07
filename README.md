# Eugene Crisis Response Data Analysis Project

This repository contains a data science analysis project focused on Eugene crisis response data. The project is organized into two Jupyter notebooks that should be run in sequence.

## Repository Contents

* `datacleaning-final.ipynb`: Initial data cleaning and preprocessing
* `data-analysis.ipynb`: Final data analysis and visualization
* `project-data`: data folder with small sample datasets to illustrate the data needed for the cleaning & analysis scripts. (TO RUN THIS PROJECT, YOU MUST DOWNLOAD YOUR DATA YOURSELF).

## Setup Instructions

1. Clone this repository to your local machine
2. Ensure you have Python 3.6+ and Jupyter Notebook/Lab installed
3. Install required dependencies:
  
      pip install pandas numpy matplotlib seaborn scikit-learn
  
4. Download the necessary datasets into the project-data folder.

DATA USED IN THIS PROJECT:

* Call data from CAD (computer-aided dispatch system), obtained via public records request from the City of Eugene Police Department, from 2014 to 2025:

This dataset has columns/variables for 'yr', 'service', 'inci_id', 'calltime', 'case_id', 'callsource', 'nature', 'closecode', 'closed_as', 'secs_to_disp', 'secs_to_arrv', 'secs_to_close', 'disp', 'arrv', 'beat', 'priority', 'zip', 'primeunit', 'units_dispd', and 'units_arrived'. Each row of the datset represents one crisis call/incident. A sample version of this dataset's structure (5 rows) is available for use in `project-data/sample_CAD_2014_data.csv`.

* Freely-available daily weather data in Eugene, OR; Downloaded from VisualCrossing.com; 2014 to 2025:

Data must be downloaded in segments. In `data-cleaning-final.ipynb` I read in separate files for 2014-01-01 to 2016-07-31, 2016-08-01 to 2018-12-31, 2019-01-01 to 2021-07-31, 2021-08-01 to 2023-12-31, and 2024-01-01 to 2025-04-07, then concatenate them together.

This dataset has columns for various weather variables, although only 'tempmax', 'tempmin', 'precip', and 'snow' are used in the final analysis.

* Freely-available daily air quality index (AQI) data in Eugene, OR; Downloaded from the EPA's Pre-Generated Data Files at https://aqs.epa.gov/aqsweb/airdata/download_files.html; 2014 to 2024

Data must be downloaded in segments by year. In `data-cleaning-final.ipynb` I read in seperate files for 2014 through 2024.

This dataset has columns/variables for 'CBSA', 'CBSA Code',	'Date', 'AQI Category', 'Defining Parameter', 'Defining Site', and 'Number of Sites Reporting'.

** Reference the file read-in code in the notebooks to organize your downloaded data in your directory accordingly, or modify the file read-in code to fit your directory's structure.**


## Running the Notebooks

Follow these steps to run the complete analysis:

1. **First:** Run `datacleaning-final.ipynb`
  
  * This will process your raw data files and generate `clean_data.csv`
  * The clean data file will be saved in the project directory
2. **Second:** Run `data-analysis.ipynb`
  
  * This notebook uses the `clean_data.csv` file created in step 1
  * For an example analysis, you can run `sample_clean_data.csv` which is a smaller dataset with the same structure that `clean_data.csv` should have.
  * This notbook performs the final analysis of the data and generates visualizations

## Important Notes

* Data must be downloaded by the user from specified sources and in the correct format to run in the notebooks.
* The notebooks must be run in the correct order as described above
* Each notebook has its own detailed README with specific instructions
* Ensure data is correctly structured, downloaded, and organized in the directory before running any notebooks
