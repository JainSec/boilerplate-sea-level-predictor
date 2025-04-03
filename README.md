# Sea Level Predictor

## Project Overview
This project analyzes global sea level changes since 1880 using historical data. The objective is to visualize the trends and predict future sea level rise through 2050 using regression analysis.

## Dataset Information
**File Name:** `epa-sea-level.csv`

| Feature | Description |
|---------|-------------|
| Year | The recorded year (X-axis) |
| CSIRO Adjusted Sea Level | The adjusted sea level measurement (Y-axis) in inches |

## Functionality
### 1. Data Processing
- Import the dataset using Pandas.
- Extract relevant columns (`Year` and `CSIRO Adjusted Sea Level`).

### 2. Scatter Plot
- **Function:** `draw_plot()`
- **Chart Details:**
  - X-axis: "Year"
  - Y-axis: "Sea Level (inches)"
  - Title: "Rise in Sea Level"
- **Visualization:** Uses Matplotlib to generate a scatter plot of sea level measurements over time.

### 3. Line of Best Fit (1880 - 2050)
- **Method:** Uses `linregress` from `scipy.stats` to calculate the slope and y-intercept.
- **Visualization:**
  - Plots a regression line from 1880 to 2050 to predict future sea level rise.

### 4. Line of Best Fit (2000 - 2050)
- **Method:** Uses `linregress` only on data from 2000 onwards to calculate a new slope and y-intercept.
- **Visualization:**
  - Plots a second regression line from 2000 to 2050 to analyze recent trends and their potential impact.

## Installation & Setup
### Requirements
- Python 3.x
- Pandas
- Matplotlib
- Scipy

### Steps
1. Clone the repository:
   ```sh
   git clone https://github.com/your-repo-url.git
   ```
2. Navigate to the project directory:
   ```sh
   cd sea-level-predictor
   ```
3. Install dependencies:
   ```sh
   pip install pandas matplotlib scipy
   ```
4. Run the script:
   ```sh
   python sea_level_predictor.py
   ```

## Example Output
- **Sea Level Prediction Plot:**
  ![Sea Level Plot Example](examples/Figure_1.png)

## Author
- Pulkit Jain
- Contact: jain.infosec@gmail.com

This is the boilerplate for the Sea Level Predictor project. Instructions for building your project can be found at https://www.freecodecamp.org/learn/data-analysis-with-python/data-analysis-with-python-projects/sea-level-predictor
