# sqlalchemy-challenge
Hawaii Weather Data Analysis

## Overview
This project aims to analyze weather data from Hawaii, specifically focusing on precipitation and temperature measurements. The data is stored in a SQLite database (`hawaii.sqlite`) containing two main tables: `measurement` and `station`. Python, along with libraries like SQLAlchemy, Pandas, and Matplotlib, is used for data retrieval, analysis, and visualization.

## Prerequisites
- Python 3.x
- Jupyter Notebook or any Python IDE
- Required Python libraries: SQLAlchemy, Matplotlib, Pandas, NumPy

## Getting Started
1. Clone this repository to your local machine.
2. Ensure you have the required Python libraries installed.
3. Open and run the Jupyter Notebook file `weather_analysis.ipynb`.

## Project Structure
- `Resources`: Contains the SQLite database file `hawaii.sqlite` where weather data is stored.
- `weather_analysis.ipynb`: Jupyter Notebook containing the Python code for data analysis and visualization.
- `app.py`: Flask application for serving weather data through API endpoints.
- `README.md`: This file providing an overview of the project and instructions.

## Data Analysis
1. **Reflect Tables into SQLAlchemy ORM**
   - Connects to the SQLite database and reflects the tables into SQLAlchemy ORM.
   - Assigns the `Measurement` and `Station` classes to variables for further querying.

2. **Exploratory Precipitation Analysis**
   - Retrieves the most recent date in the dataset.
   - Calculates the date one year prior to the most recent date.
   - Queries precipitation data for the last 12 months and plots the results using Matplotlib.
   - Calculates summary statistics for the precipitation data.

3. **Exploratory Station Analysis**
   - Calculates the total number of stations in the dataset.
   - Identifies the most active stations based on the number of data entries.
   - Calculates the lowest, highest, and average temperature for the most active station.
   - Queries the last 12 months of temperature observation data for the most active station and plots the results as a histogram.

4. **Flask API Development**
   - Implements a Flask application to serve weather data through API endpoints.
   - Provides endpoints for retrieving precipitation, station information, temperature observations, and temperature statistics.

5. **Conclusion**
   - This project provides valuable insights into the weather patterns of Hawaii, including precipitation levels and temperature variations. The analysis and visualizations can be further extended for more in-depth studies or integrated into larger applications.

## Usage
To run the Flask application:
1. Open a terminal or command prompt.
2. Navigate to the project directory.
3. Run the command `python app.py`.
4. Access the API endpoints as described in the Flask Routes section of `app.py`.

## Acknowledgments
- Dataset provided from external sources.
- Inspiration and guidance from the SQLAlchemy and Flask documentation.
