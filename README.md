# Python-IMDb-MovieData-WebScraping
This repository uses BeautifulSoup and Selenium. It processes and stores movie details such as titles, release years, and ratings into a structured CSV format. This project demonstrates skills in web scraping, data processing, and Python programming, and serves as a resource for data analysis and visualization in the movie domain.

### **`TOPIC`**: Web scraper for IMDb website

#### **`INTRODUCTION`**

This project aims to scrape to top 250 movies of all time from IMDb website: https://www.imdb.com/chart/top/?ref_=nv_mv_250 

IMDb, founded in 1990, has grown to become one of the most comprehensive and authoritative platforms for information related to films, television shows, and the people who bring them to life. With its vast database of movie details, actor biographies, user-generated reviews, and ratings, IMDb has become a go-to source for moviegoers and researchers.

The purpose of this report is to present findings and insights obtained through web scraping IMDb's website. The following details about each movie has been scraped: 

*   Movie Title
*   Movie Release Year
*   IMDb Rating out of 10
*   Movie Duration
*   Movie Rating (What audience is it appropriate for)
*   Movie URL

Through this project, we aim to showcase the power of web scraping as a tool for data extraction and analysis in the context of a popular online database like IMDb.

#### **`METHODOLOGY`**

This project uses the following Python libraries:

| Library/Module                                      | Purpose                                             |
| --------------------------------------------------- | --------------------------------------------------- |
| Requests                                            | To send HTTP requests and retrieve web pages        |
| BeautifulSoup (from bs4)                            | To parse and navigate HTML content                  |
| CSV                                                 | To read and write CSV files                         |
| Pandas                                              | To manipulate and analyze data using data frames    |
| Time                                                | To introduce delays and manage time-related operations |
| urllib.parse (from urllib.parse)                    | To handle URL manipulation and joining             |
| Selenium Webdriver                                  | To automate web interactions and access websites    |
| Chrome Options (from selenium.webdriver.chrome.options) | To configure the Chrome WebDriver                   |
| By (from selenium.webdriver.common.by)              | To locate elements on web pages using various methods |



#### **`ENVIRONMENT SETUP`**

You will need to install the following Python Libraries: 

`pip install requests beautifulsoup4 pandas selenium`

Additionally, you will need to download and configure the Chrome WebDriver separately for Selenium as mentioned earlier.


#### **`TOOLS USED`**

*   Chrome Browser
*   Jupyter Notebook
*   Python 3.11.2


#### **`SOLUTION`**

In this project, we successfully scraped data from IMDb's list of the top 250 movies of all time. We used a combination of two powerful Python libraries, Requests and BeautifulSoup, to fetch and parse the initial HTML page. Then, we utilized Selenium WebDriver to handle dynamic web content and collect additional data. Here's a brief overview of the solution:


#### **Data Collection:**
In the IMDb scraping project, data collection is the initial step where we gather information from IMDb's website. IMDb, short for the Internet Movie Database, is a popular online database of movies, TV shows, and celebrities. It provides a wealth of information about films, including movie titles, release years, ratings, and more.


#### **Web Page Rendering:**
After selecting IMDb as our data source, the next step is web page rendering. In this project, we use Selenium, a powerful tool for automating web interactions, to render IMDb's web pages. Rendering involves opening a web page using a web browser, in this case, Chrome, and allowing it to fully load. This is crucial because IMDb's website uses JavaScript to load dynamic content, such as movie ratings and details, which isn't present in the initial HTML response. By rendering the page, we ensure that all data is available for extraction.


#### **HTML Parsing:**
With the rendered web page at our disposal, we employ BeautifulSoup, a Python library, to parse the HTML content. 


#### **Data Extraction:**
Data extraction is the heart of the project. We identify and target specific HTML elements on the IMDb web page that contain the information we want. In this case, we extract movie titles, release years, IMDb ratings, movie durations, and movie URLs. To achieve this, we use techniques like CSS selectors to pinpoint the exact location of the desired data within the HTML structure.


#### **Data Validation and Handling:**
Data validation and handling ensure that the extracted data is of high quality and consistency. For instance, if a movie's release year is not available on the web page, we assign it the value "Not Provided" to indicate that the information is missing. This step is vital for maintaining data integrity and ensuring that the resulting dataset is clean and ready for analysis.


#### **CSV File Creation:**
Once we have successfully extracted and validated the data, the final step is to create a structured format for storage. We use Python's Pandas library to organize the data into a DataFrame, a tabular data structure. This DataFrame is then saved as a CSV (Comma-Separated Values) file. 


#### **`PROJECT CONCLUSION`** 

The project concludes with a final message that indicates that the CSV file was successfully created.
The CSV file can be further analysed or used for various purposes, such as data analysis, reporting, or data visualization.


#### **`REFERENCES`** 

1. Reference Notebook provided by the professor to scrape Indeed
2. ChatGPT 3.5: for helping to solve errors

