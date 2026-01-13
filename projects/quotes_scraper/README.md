# Quotes Scraper (quotes.toscrape.com)

This project scrapes quotes from **https://quotes.toscrape.com/** and saves them into a CSV file using **Requests**, **BeautifulSoup**, and **Pandas**.

## What it scrapes
For each quote, it extracts:
- **Quote text**
- **Author name**
- **Author profile link** (relative path like `/author/Albert-Einstein`)
- **Tags** (comma-separated)

## Output
A CSV file like:

- `Quotes.csv`

Columns:
- `quote`
- `author`
- `author_id`
- `tags`
- (optional) `author_link` (full URL)

## Files in this repo
- `Page_Scrapper.ipynb` → scrapes quotes from the page
- `Scraping_Articles_with_author.ipynb` → author link building / extra scraping
- `Quotes.csv` → scraped output
- `main.html` → saved HTML page (optional)

## Installation
Create a virtual environment and install required packages:

```bash
pip install -r requirements.txt
