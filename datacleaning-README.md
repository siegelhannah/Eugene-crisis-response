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

1. Extract the raw data files:
  
  * Navigate to the `project-data` folder
  * Extract the contents of `zipped-raw-data.zip` in the same directory
  * Verify that all raw data files are now accessible
2. Install required dependencies:
  
      pip install pandas numpy matplotlib
  

## Running the Notebook

1. Launch Jupyter Notebook/Lab in your project directory:
  
      jupyter notebook
  
  or
  
      jupyter lab
  
2. Open `datacleaning-script.ipynb` from the Jupyter interface
  
3. Run all cells in sequence
  
  * The notebook includes detailed markdown cells explaining each step
  * Monitor cell execution for any warnings or errors

## Output

The notebook will generate:

* `clean_data.csv`: A cleaned and preprocessed dataset that will be used by the subsequent notebooks
* This file will be saved in the project root directory

## Important Notes

* This notebook must be run before the EDA and analysis notebooks
* The `clean_data.csv` file is required for the subsequent notebooks to function
* Running time may vary depending on the size of the raw data files
* If you encounter any data path issues, ensure that the raw data files are correctly extracted from the zip file
