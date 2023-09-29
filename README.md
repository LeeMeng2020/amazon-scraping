# amazon-scraping
**Web Scraper sitemaps for scraping Amazon, updated for 2023**

These are sitemaps (scripts) for use with the Web Scraper extension from https://webscraper.io/

These should not to be confused with the typical sitemaps used for websites.

## amazon-reviews-scraper.json

Scrapes reviews for specific products on Amazon.
- Handles pagination. Set to stop at page 3 (limiter). This can be changed by modifying 
  the number in the paginator's click selector:
  <br>`div > ul.a-pagination li.a-last:not([a-disabled]) a:not([href*='paging_btm_4'])`
  <br>To remove the limiter, just delete the `:not` condition, leaving only:
  <br>`div > ul.a-pagination li.a-last:not([a-disabled]) a`
- Sample result file: amazon-reviews-scraper.csv

## amazon-electronics.json

Scrapes product details from the electronics section on Amazon.
- Handles pagination. Set to stop at page 4 (limiter). This can be changed by modifying 
  the number in the paginator's click selector:
  <br>`div[role='navigation'] a.s-pagination-next:not([aria-label$='page 5'])`
  <br>To remove the limiter, just delete the `:not` condition, leaving only:
  <br>`div[role='navigation'] a.s-pagination-next`
- Clicks through to each product detail page.
- Sample result file: amazon-electronics.csv

## amazon-bestsellers-books-paginate.json

Scrapes Amazon book bestsellers.
- Handles pagination.
- Includes scroller to deal with lazy-loading.
- Tested with Amazon US, UK, and Canada.
- Sample result file: amazon-bestsellers-books-paginate.csv
