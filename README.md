# iHerb_Hair_Care_Product_Analysis_2024

## Background
This project investigates the best-selling hair care products on iHerb, aiming to analyze consumer preferences and market trends through data-driven methods. We utilized web scraping techniques to gather comprehensive product information and customer reviews, focusing on 630 products across various categories.

## Scope
Our analysis encompasses several key components:

- **Web Scraping**: Using tools like Selenium and BeautifulSoup, we collected data while overcoming anti-crawler measures implemented by iHerb.
  
- **Data Preprocessing**: The scraped data underwent rigorous cleaning and standardization to ensure accuracy and usability.
  
- **Exploratory Data Analysis (EDA)**: We employed visualizations to identify trends in sales performance, product distribution, and correlations among different variables.
  
- **Sentiment Analysis**: By leveraging Natural Language Processing (NLP) techniques, we analyzed customer sentiments expressed in reviews to gain insights into consumer behavior.

The findings reveal significant trends, such as the dominance of brands like Mielle and SheaMoisture in sales, while highlighting areas for potential growth, particularly for underperforming brands like Dove. This project not only sheds light on current market dynamics but also lays the groundwork for future research into consumer preferences in the hair care industry.

## Language & Tools
The scripts are developed using **Python**, and the data visualization and analysis are conducted with **Power BI**.

## Notebook and Data Files

### Data Files
- **iHerb_hair_care_raw_dataset.csv**: This CSV file contains the web scraped product information, including details on various hair care products from iHerb.

- **iHerb_hair_care_clean_dataset.csv**: This file contains the cleansed data, prepared for visualization and analysis.

- **product_name_split.csv**: A dataset containing split product names for more detailed analysis.

- **reviews_raw_dataset.csv**: This file includes the scraped customer reviews.

- **reviews_clean_dataset.csv**: A cleansed dataset of customer reviews, intended for generating word clouds and further analysis.

### Notebooks
- **01_data_extraction_web_scraping.ipynb**: This notebook performs web scraping to create the `iHerb_hair_care_raw_dataset.csv` output.

- **02_data_preprocessing_exploration.ipynb**: A Jupyter notebook for cleaning and preprocessing the `iHerb_hair_care_raw_dataset.csv`, as well as performing exploratory data analysis (EDA). The output is the `iHerb_hair_care_clean_dataset.csv`, which can be used for developing dashboards with Power BI.

- **03_sentiment_analysis_VADER_RoBERTa.ipynb**: This notebook focuses on analyzing customer reviews using Natural Language Processing (NLP) techniques to gauge sentiment and consumer behavior.

## Web Driver

### Edge Browser Driver
This project utilizes the Microsoft Edge browser for web scraping with Selenium. To facilitate this, the appropriate Edge WebDriver must be installed and configured.

- **Driver File**: The Edge browser driver is included in this repository for reference. Ensure that the driver version matches your installed version of the Edge browser.

### Setup Instructions
1. **Download Edge WebDriver**: If you need to update or install the driver, you can download the correct version from the [Microsoft Edge WebDriver page](https://developer.microsoft.com/en-us/microsoft-edge/tools/webdriver/).

2. **Configure PATH**: Ensure that the WebDriver executable is in your system's PATH, or specify the driver path directly in your scripts.
   
   Example:
   ```python
   from selenium import webdriver

   driver = webdriver.Edge(executable_path='path/to/msedgedriver')
