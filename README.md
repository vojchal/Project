# Python Project: Interactive Stock Analysis with ARMA-GARCH

This is a Python project built in **Jupyter Lab** for interactive stock data analysis. The project allows users to select groups of stocks, choose specific tickers, perform basic statistical analysis, visualize price and return data, and run **ARMA-GARCH modeling** on selected stocks.

---

## Features

1. **Environment Check**
   - Automatically checks if all required Python packages are installed.
   - Offers to install missing packages.

2. **Stock Group Selection**
   - Select from predefined groups: `ALL`, `NASDAQ`, `NYSE`, `SP500`.
   - Checks availability of tickers on Yahoo Finance.
   - Saves the available tickers in a CSV file.

3. **Ticker Selection and Basic Analysis**
   - Enter up to 4 tickers manually, or choose random tickers from the group.
   - Downloads historical stock data from Yahoo Finance.
   - Generates CSV files for each selected ticker.
   - Provides interactive visualizations:
     - Daily close prices (2 months and 2 years)
     - Logarithmic returns distribution
     - Descriptive statistics

4. **ARMA-GARCH Modeling**
   - Fits ARMA(p,q) and GARCH(p,q) models for each selected ticker.
   - Automatically selects best model parameters based on AIC.
   - Visualizes log returns, fitted ARMA mean, and GARCH volatility with 95% confidence intervals.

5. **CSV File Management**
   - Interactive tool to delete selected CSV files from the working directory.

---
  
## Instructions

1. **Download the project**
   - Download `Scripts.zip` from this GitHub repository.
   - Extract the ZIP file to a folder of your choice.
   - Make sure **all files** remain together in one folder - the project relies on the folder structure for imports.

2. **Open in Jupyter Lab**
   - Launch **Jupyter Lab** and navigate to the folder with the extracted files.
   - Open `Main_script.ipynb`. This is the main interface, which guides you step by step through the stock analysis process.

3. **Install required packages**
   - You can install all dependencies using the provided `requirements.txt` by running in :
     ```bash
     pip install -r requirements.txt
     ```
   - Alternatively, the `Main_script.ipynb` will automatically check for missing packages and offer to install them for you at the start.

4. **Run the analysis**
   - Follow the instructions inside the script. 

---

## Notes

- Internet connection is required to download stock data from Yahoo Finance.
- For S&P 500 tickers, additional company information is retrieved from Wikipedia, along with clickable links to the relevant Wiki pages.
