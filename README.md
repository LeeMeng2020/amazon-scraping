# amazon-scraping
**Web Scraper sitemaps for scraping Amazon, updated for 2023**

These are sitemaps (scripts) for use with the Web Scraper extension from https://webscraper.io/

These should not to be confused with the typical sitemaps used for websites.

## amazon-bestsellers-books-paginate.json

Scrapes Amazon book bestsellers.
- Handles pagination.
- Includes scroller to deal with lazy-loading.
- Tested with Amazon US, UK, and Canada.
- Sample result file: amazon-bestsellers-books-paginate.csv

## amazon-reviews-scraper.json

Scrapes reviews for specific products on Amazon.
- Handles pagination. Set to stop at page 3. This can be changed.
- Sample result file: amazon-reviews-scraper.csv

## amazon-electronics.json

Scrapes product details from the electronics section on Amazon.
- Handles pagination. Set to stop at page 4. This can be changed.
- Clicks through to each product detail page.
- Sample result file: amazon-electronics.csv
