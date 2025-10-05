This repository contains two web scraping projects that use the Python library BeautifulSoup to extract data from websites. The first project scrapes financial data of the top 100 US companies, and the second one scrapes news articles from India.

American Revenue Scrapping
This project extracts data from the Wikipedia page "List of largest companies in the United States by revenue".

Dataset: CompaniesRevenueData.csv

The data is stored in CompaniesRevenueData.csv and includes the following columns:

Rank: The company's rank by revenue.

Name: The official name of the company.

Industry: The primary industry in which the company operates.

Revenue (USD millions): The company's total revenue in millions of US dollars.

Revenue growth: The percentage of revenue growth over the previous period.

Employees: The total number of employees at the company.

Headquarters: The city and state of the company's main headquarters.

India News Scrapping
This project scrapes news articles related to India and saves them in a CSV file.

Dataset: IndiaNews.csv

The data is stored in IndiaNews.csv and includes the following columns:

webTitle: The title of the news article.

sctionName: The section of the news source where the article was published (e.g., Politics, World news).

publishdate: The date and time the article was published.

url: The URL of the news article.

Why BeautifulSoup over Selenium?
For the web scraping tasks in this repository, BeautifulSoup is the ideal choice over a browser automation tool like Selenium. Here's why:

Efficiency: BeautifulSoup is significantly faster and uses fewer system resources than Selenium. This is because it only parses the HTML content of a page and does not need to load a full web browser.

Simplicity: For scraping static websites where the data is readily available in the page's HTML, BeautifulSoup provides a simple and direct way to access the data.

No Need for Browser Automation: Selenium is designed for dynamic websites where content is loaded and rendered using JavaScript. Since the data for both projects in this repository is present in the initial HTML, the browser automation capabilities of Selenium are not needed.

How to Use This Repository
Clone the repository:

Bash

git clone https://github.com/tushhhaarrr/beautifulscrapping.git
Install the required libraries:

Bash

pip install -r requirements.txt
Run the Jupyter Notebooks:

To run the American Revenue Scrapping project, open and run the cells in AmericanREvenue Scrapping/WikipediaScrapping.ipynb.

To run the News Scrapping project, you will need to create a similar Jupyter Notebook in the NewsScrapping directory that scrapes the news source of your choice.

Contributing
Contributions to this project are welcome. Please feel free to fork the repository, make your changes, and submit a pull request.
