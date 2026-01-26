Quotes Scraper

A simple Python web scraper that collects quotes, authors, and categories from
https://quotes.toscrape.com
.

The script automatically:

Detects all categories

Scrapes all quotes per category

Handles pagination

Exports results to a CSV file

Tech Stack

Python

requests

BeautifulSoup

Usage
pip install requests beautifulsoup4
python scraper.py

Output

all_quotes.csv containing:

category

quote

author

Disclaimer

For educational purposes only
