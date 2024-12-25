Product List Crawler

This script crawls a list of product URLs from a given domain using asynchronous requests and Selenium as a fallback for JavaScript-rendered pages.

Usage

Install the required libraries: aiohttp, beautifulsoup4, selenium, and webdriver-manager.
Update the domains list with the URLs you want to crawl.
Run the script using python productlist.ipynb.
Functionality

The script uses the following functions:

init_selenium(): Initializes a Selenium WebDriver instance.
fetch_links(): Fetches links from a given URL using asynchronous requests.
fetch_links_selenium(): Fetches links from a given URL using Selenium as a fallback.
filter_product_urls(): Filters product URLs from a list of links.
crawl_domain(): Crawls a domain and extracts product URLs.
main(): Orchestrates the crawling process and saves the results to a JSON file.
Output

The script saves the crawled product URLs to a JSON file named product_urls.json.

Notes

Make sure to update the domains list with the URLs you want to crawl.
The script uses Selenium as a fallback for JavaScript-rendered pages, so make sure you have the correct WebDriver installed.
The script saves the results to a JSON file, so make sure you have the necessary permissions to write to the file.
