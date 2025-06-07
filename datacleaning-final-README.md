# Data Cleaning Script

This Jupyter notebook performs the initial data cleaning and preprocessing for the Eugene crisis response data analysis project.

## Prerequisites

* Python 3.6+
* Jupyter Notebook/Lab
* Required libraries:
  * pandas
  * numpy
  * matplotlib (for optional visualizations)

## Setup Instructions

1. Obtain the raw data files:

* Call data from CAD (computer-aided dispatch system). A sample version of this dataset's structure (5 rows) is available for use in `project-data/sample_CAD_2014_data.csv`.

* Freely-available daily weather data in Eugene, OR; Downloaded from VisualCrossing.com; 2014 to 2025: Data must be downloaded in segments. In `data-cleaning-final.ipynb` I read in separate files for 2014-01-01 to 2016-07-31, 2016-08-01 to 2018-12-31, 2019-01-01 to 2021-07-31, 2021-08-01 to 2023-12-31, and 2024-01-01 to 2025-04-07, then concatenate them together.

* Freely-available daily air quality index (AQI) data in Eugene, OR; Downloaded from the EPA's Pre-Generated Data Files at https://aqs.epa.gov/aqsweb/airdata/download_files.html; 2014 to 2024. Data must be downloaded in segments by year. In `data-cleaning-final.ipynb` I read in seperate files for 2014 through 2024.

** Reference the file read-in code in the notebooks to organize your downloaded data in your directory accordingly, or modify the file read-in code to fit your directory's structure.**


2. Install required dependencies:
  
      pip install pandas numpy matplotlib
  

## Running the Notebook

1. Launch Jupyter Notebook/Lab in your project directory:
  
      jupyter notebook
  
  or
  
      jupyter lab
  
2. Open `datacleaning-final.ipynb` from the Jupyter interface
  
3. Run all cells in sequence
  
  * The notebook includes detailed markdown cells explaining each step
  * Monitor cell execution for any warnings or errors

## Output

The notebook will generate:

* `clean_data.csv`: A cleaned and preprocessed dataset that will be used by the subsequent notebooks
* This file will be saved in the project root directory

## Important Notes

* This notebook must be run before the analysis notebook
* The `clean_data.csv` file is required for the other notebook to function
* Running time may vary depending on the size of the raw data files
* If you encounter any data path issues, ensure that the raw data files are correctly extracted from the zip file
