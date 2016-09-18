# Open Data Projects with Python

Learning to program can be easier when you have a problem to solve. The notebooks here are simple examples of working with open data to answer real world questions or problems.

This material was originally written for [PyConUK 2016](http://2016.pyconuk.org/workshops/open-data-projects-with-python/), and the accompanying presentation is [here](https://github.com/pwalsh/presentations/tree/master/opendataprojects).

## Skill level

The notebooks here are designed for those new to programming, and learning with Python.

Ideally, you'll be comfortable with the basics of Python syntax, and very basic debugging.

If you need a primer, start working through [Learn Python the Hard Way](http://learnpythonthehardway.org).

## What you need

You need Python 3 installed, and then:

- `git clone git@github.com:pwalsh/notebooks.git`
- `cd notebooks/opendataprojects`
- `pip install --upgrade -r requirements.txt`
- `jupyter notebook`

## Dependencies

The dependencies are installed with `pip install --upgrade -r requirements.txt`.

There are 4 key dependencies; all are powerful libraries that are worth deeper investigation.

### bokeh

So that we can embed visualisations right into our notebooks.

- [Documentation](http://bokeh.pydata.org)
- [Source code](https://github.com/bokeh/bokeh)
- [Tutorial](http://bokeh.pydata.org/en/0.11.1/docs/user_guide/charts.html)

### jupyter

So that we can use Jupyter notebooks, and build a narrative with code, text, and visuals.

- [Documentation](https://jupyter.readthedocs.io)
- [Source code](https://github.com/jupyter/jupyter)
- [Tutorial](https://jupyter-notebook-beginner-guide.readthedocs.io/en/latest/)

### pyquery

A great library for working with HTML pages, and a more than capable tool for basic scraping.

- [Documentation](http://pyquery.readthedocs.io)
- [Source code](https://github.com/gawel/pyquery)
- [Tutorial](http://davedash.com/tutorial/pyquery/)

### requests

A clean and simple library for making http requests.

- [Documentation](http://docs.python-requests.org)
- [Source code](https://github.com/kennethreitz/requests)
- [Tutorial](http://docs.python-requests.org/en/master/user/quickstart/)

## Defining a problem

You'll find here some notebooks that seek to answer some simple 'problems' with open data.

The whole point of these examples to to help you find a starting point to answer your own questions.

However, if you are having trouble finding a place to start, here are some questions and problems to get you going.

## Ideas

1. How is money from the EU distributed throughout the UK?
2. Is government spending on infrastructure for schooling consistent per capita across the UK?
3. Is expenditure on defence on the increase?
4. Is there a correlation between declining industry (pick any) and unemployment (per region?)?
5. Do hospital beds correspond to the area the hospital serves? Is there a relationship between hospital bed availability and socioeconomic indicators?

## Resources

- http://ons.gov.uk
- https://data.gov.uk
- https://github.com/datasets
- https://aws.amazon.com/public-data-sets/
- https://www.data.gov
- http://ec.europa.eu/eurostat
- https://www.iatiregistry.org
- https://data.humdata.org

And so much more.

## Troubleshooting

- working with text files can be complicated due to file encoding issues. Use [chardet](http://chardet.readthedocs.io/en/latest/usage.html) to detect a file's encoding if you are having problems.
- data from text files often uses strings like 'n/a' or 'null' to represent 'no value'. When iterating over data, normalise such strings.
