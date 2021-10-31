# BudapestBI FugueSQL presentation

[![Kaggle](https://img.shields.io/badge/launch-kaggle-blue)](https://www.kaggle.com/rdmolony/2021-10-budapestbi-fuguesql-workshop)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/rdmolony/demos/blob/main/2021-10-budapestbi-fuguesql/workshop.ipynb)
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/rdmolony/demos/HEAD?labpath=2021-10-budapestbi-fuguesql%2Fworkshop.ipynb)

> Developed in partnership with @kvnkho

In this session we will be introduce FugueSQL, a language that allows heavy SQL users to work on Python-based DataFrames.

FugueSQL allows users to express computation workflows with a SQL-like interface. This code is then parsed and executed on any of the Pandas, Spark, and Dask engines. To provide a rich grammar for handling data, FugueSQL has enhancements over ANSI SQL such as keywords specific to distributed computing (PERSIST, BROADCAST, PARTITION), as well as support for custom Python functions. These allow users to leverage distributed computing, while using a language that they are already familiar with.

See [budapestbi](https://budapestbi.hu/2021/eloadok/kevin-kho/)
