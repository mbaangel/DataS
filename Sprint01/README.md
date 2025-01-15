# Sprint project
> E-Commerce Data Pipeline

The first of several projects we're going to be working on.


## The Business problem

You are working for one of the largest E-commerce sites in Latam and they requested the Data Science team to analyze company data to understand better their performance in specific metrics during the years 2016-2018.

They are two main areas they want to explore, those are **Revenue** and *Delivery*.

Basically, they would like to understand how much revenue by year they got, which were the most and less popular product categories, and the revenue by state. On the other hand, it's also important to know how well the company is delivering the products sold in time and form to their users. For example, seeing how much takes to deliver a package depends on the month and the difference between the estimated delivery date and the real one.

## About the data

You will consume and use data from two sources.

The first one is a Brazilian e-commerce public dataset of orders made at the Olist Store, provided as CSVs files. This is real commercial data, that has been anonymized.

The second source is a public API: https://date.nager.at. You will use it to retrieve information about Brazil's Public Holidays and correlate that with certain metrics about the delivery of products.

## Technical aspects

Because the team knows the data will come from different sources and formats, also, probably you will have to provide these kinds of reports on a monthly or annual basis. They decided to build a data pipeline (ELT) they can execute from time to time to produce the results.

The technologies involved are:
- Python as the main programming language
- Pandas for consuming data from CSVs files
- Requests for querying the public holidays API
- SQLite as a database engine
- SQL as the main language for storing, manipulating, and retrieving data in our Data Warehouse
- Matplotlib and Seaborn for the visualizations
- Jupyter notebooks to make the report an interactive way

## Instalation

A `requirements.txt` file is provided with all the needed Python libraries for running this project. For installing the dependencies just run:

```console
$ pip install -r requirements.txt
```

*Note:* We encourage you to install those inside a virtual environment.

## Code Style

Following a style guide keeps the code's aesthetics clean and improves readability, making contributions and code reviews easier. Automated Python code formatters make sure your codebase stays in a consistent style without any manual work on your end. If adhering to a specific style of coding is important to you, employing an automated to do that job is the obvious thing to do. This avoids bike-shedding on nitpicks during code reviews, saving you an enormous amount of time overall.

We use [Black](https://black.readthedocs.io/) for automated code formatting in this project, you can run it with:

```console
$ black --line-length=88 .
```

Wanna read more about Python code style and good practices? Please see:
- [The Hitchhiker’s Guide to Python: Code Style](https://docs.python-guide.org/writing/style/)
- [Google Python Style Guide](https://google.github.io/styleguide/pyguide.html)

## Tests

We provide unit tests along with the project that you can run and check from your side the code meets the minimum requirements of correctness needed to approve. To run just execute:

```console
$ pytest tests/
```

If you want to learn more about testing Python code, please read:
- [Effective Python Testing With Pytest](https://realpython.com/pytest-python-testing/)
- [The Hitchhiker’s Guide to Python: Testing Your Code](https://docs.python-guide.org/writing/tests/)
