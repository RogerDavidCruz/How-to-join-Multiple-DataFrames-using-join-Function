# Guided Lab 386.4.3 – Joining Multiple Pandas DataFrames

## Overview

This lab introduces how to combine Pandas DataFrames using the `.join()` function. It demonstrates joining DataFrames by index, applying different join types, joining on columns, and handling overlapping column names.

## Objectives

* Use the Pandas `.join()` function
* Join DataFrames by row index
* Perform left, inner, and right joins
* Join DataFrames using a column
* Handle overlapping column names
* Preserve the original DataFrame index

## Technologies Used

* Python 3
* Pandas
* Google Colab / Jupyter Notebook

## Methods & Concepts

* `DataFrame.join()` – Combine DataFrames using indexes by default
* `how='left'` – Keep all rows from the left DataFrame
* `how='inner'` – Keep only rows with matching indexes
* `how='right'` – Keep all rows from the right DataFrame
* `on='column'` – Join using a column from the left DataFrame
* `set_index()` – Convert a column into the DataFrame index
* `lsuffix` – Add a suffix to overlapping columns from the left DataFrame
* `rsuffix` – Add a suffix to overlapping columns from the right DataFrame
* `.shape` – Check the number of rows and columns after the join

## Key Points

* `.join()` performs a left join on indexes by default.
* Unmatched values are filled with `NaN`.
* Inner joins remove rows without matching indexes.
* Right joins keep every row from the right DataFrame.
* Columns can be used as join keys by converting them into indexes.
* Suffixes are required when both DataFrames contain columns with the same name.

## Topics Covered

* Index-based DataFrame joins
* Left joins
* Inner joins
* Right joins
* Joining on columns
* Setting columns as indexes
* Handling overlapping column names
* Preserving the original index
* Comparing DataFrame dimensions after joining

## Dataset

* Sample technology course DataFrames created from Python dictionaries

## Learning Outcome

By completing this lab, I gained hands-on experience joining Pandas DataFrames by indexes and columns, applying different join types, handling overlapping column names, and managing unmatched values in combined datasets.
