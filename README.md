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

### Scraping Walmart

Website [Walmart](https://www.walmart.ca/)
Category: Groceries
Branches: `3124` and `3106`

Go to the backend-integration-test in the command prompt

Scrapy:

```sh
$ scrapy crawl ca_walmart
```
