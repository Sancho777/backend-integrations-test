# Cornershop's backend integrations test

## Installation

Make sure that you have installed Python 3.6.9 (https://www.python.org/)

### Start project

Create a virtual environment

```sh
$ python3 -m venv venv
```

Active virtual environment

```sh
$ source venv/bin/activate
```

Install packages

```sh
$ pip install -r requirements.txt
```

### Richart's Wholesale Club

Make directory called `dataset` y save following files:

- [PRODUCTS.csv](https://cornershop-scrapers-evaluation.s3.amazonaws.com/public/PRODUCTS.csv): Contains the products basic information

- [BRANCHES.csv](https://cornershop-scrapers-evaluation.s3.amazonaws.com/public/BRANCHES.csv): Contains information about the branches

- [PRICES.csv](https://cornershop-scrapers-evaluation.s3.amazonaws.com/public/PRICES.csv): Contains information about the prices

- [STOCK.csv](https://cornershop-scrapers-evaluation.s3.amazonaws.com/public/STOCK.csv): Contains information about the stock

To process the csv files and save it in sqlite database run:

For all products

```sh
$ python main.py
```

For 500 products

```sh
$ python main.py -p 500
```

### Scraping Walmart

Website [Walmart](https://www.walmart.ca/)
Category: Groceries
Branches: `3124` and `3106`

```sh
$ scrapy crawl walmart_crawler
```
