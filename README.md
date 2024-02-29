# Selenium_WS

# Web Scraping with Selenium and BeautifulSoup

This script uses Selenium and BeautifulSoup to scrape a web page, find instances of a specified keyword, and save the results in a text file.

## Prerequisites
- Python installed on your system
- Required Python packages: selenium, beautifulsoup4, webdriver_manager


## steps:

1. **Initialize WebDriver:**
   - The script uses ChromeDriver managed by `webdriver_manager` to initialize the Selenium WebDriver.

2. **User Input:**
   - Prompt the user to enter a URL.

3. **Load Page:**
   - Open the provided URL in the browser and wait for it to fully load.

4. **Extract Page Source:**
   - If the loaded URL matches the entered URL, extract the page source.

5. **Parse HTML:**
   - Use BeautifulSoup to parse the HTML page source.

6. **Find Instances of Keyword:**
   - Prompt the user to enter a keyword to search for in the article.
   - Find all instances of the keyword within the HTML body using regular expressions.

7. **Write Results to File:**
   - Write the title of the page to a text file (`text_scraping.txt`).
   - Write all instances of the keyword found in the article to the file, along with a count.
   - Close the file.

8. **Clean Up:**
   - Quit the WebDriver.
