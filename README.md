Material for Data Quality in a Data Engineering perspective
===========================================================

# Table of Content (ToC)
* [Overview](#overview)
* [References](#references)
  * [Articles](#articles)
    * [Data Quality with Great Expectations](#data-quality-with-great-expectations)
    * [Data validation, documentation, and profiling](#data-validation-documentation-and-profiling)
    * [Preventing data quality issues with unit testing](#preventing-data-quality-issues-with-unit-testing)
    * [Data Quality in Python Pipelines](#data-quality-in-python-pipelines)
    * [Using data linter to streamline data quality checks](#using-data-linter-to-streamline-data-quality-checks)
    * [Concepts and practices to ensure data quality](#concepts-and-practices-to-ensure-data-quality)
    * [Stop Firefighting Data Quality Issues](#stop-firefighting-data-quality-issues)
    * [The four pillars of data observability](#the-four-pillars-of-data-observability)
    * [Data Quality Validation for Python Dataframes](#data-quality-validation-for-python-dataframes)
* [Frameworks and tools](#frameworks-and-tools)
  * [Deequ](#deequ)
  * [Great Expectations (GX)](#great-expectations-gx)
  * [Data Diff](#data-diff)
  * [Elementary](#elementary)
  * [SODA](#soda)
  * [Pydantic](#pydantic)

Created by [gh-md-toc](https://github.com/ekalinin/github-markdown-toc.go)


# Overview
[This project](https://github.com/data-engineering-helpers/data-quality)
intends to document requirements and referential material to improve
data quality through implementation of data validation rules
in the perspective of data engineering on a modern data stack (MDS).

Even though the members of the GitHub organization may be employed by
some companies, they speak on their personal behalf and do not represent
these companies.

# References
* [Material for Data platform - Data contracts](https://github.com/data-engineering-helpers/data-contracts)
* [Architecture principles for data engineering pipelines on the Modern Data Stack (MDS)](https://github.com/data-engineering-helpers/architecture-principles)
  + [Material for the Data platform - Architecture principles](https://github.com/data-engineering-helpers/architecture-principles/blob/main/material/README.md)
* Specifications/principles for a
  [data engineering pipeline deployment tool](https://github.com/data-engineering-helpers/data-pipeline-deployment)

## Articles

### Data Quality with Great Expectations
* Title: Data Quality with Great Expectations
* Date: May 2023
* Author: Charles Verleyen
  ([Charles Verleyen on LinkedIn](https://www.linkedin.com/in/charlesverleyen/),
   [Charles Verleyen on Medium](https://medium.com/@charles.xavier.verleyen))
* Link to the article:
  https://medium.astrafy.io/data-quality-with-great-expectations-e41504d93e17
* Publisher: Medium

### Data validation, documentation, and profiling
* Title: Data Validation, Documentation, and Profiling with Great Expectations
* Date: March 2023
* Author: Seckin Dinc
  ([Seckin Dinc on LinkedIn](https://www.linkedin.com/in/seckindinc/),
   [Seckin Dinc on Medium](https://medium.com/@seckindinc))
* Link to the article:
   https://medium.com/@seckindinc/data-validation-documentation-and-profiling-with-great-expectations-c7d05690c690
* Publisher: Medium

### Preventing data quality issues with unit testing
* Title: Preventing Data Quality Issues with Unit Testing
* Date: March 2023
* Author: Seckin Dinc
  ([Seckin Dinc on LinkedIn](https://www.linkedin.com/in/seckindinc/),
  [Seckin Dinc on Medium](https://medium.com/@seckindinc))
* Link to the article:
   https://medium.com/@seckindinc/preventing-data-quality-issues-with-unit-testing-1b0565d3a4db
* Publisher: Medium

### Data Quality in Python Pipelines
* Title: Data Quality in Python Pipelines!
* Date: March 2023
* Author: Josue Luzardo Gebrim
  ([Josue Luzardo Gebrim on LinkedIn](https://www.linkedin.com/in/josueluzardo/),
   [Josue Luzardo Gebrim on Medium](https://jlgjosue.medium.com/))
* Link to the article:
   https://jlgjosue.medium.com/data-quality-in-python-pipelines-4ad1e8eb6603
* Publisher: Medium

### Using data linter to streamline data quality checks
* Title: Using Data Linter to Streamline Data Quality Check
* Date: March 2023
* Author: Victoria Jiang
  ([Victoria Jiang on LinkedIn](https://www.linkedin.com/in/victoria-jiang-034953129/),
   [Victoria Jiang on Medium](https://medium.com/@shuyuj))
* Link to the article:
   https://medium.com/@shuyuj/using-data-linter-to-streamline-data-quality-check-490a1eb6cdd6
* Publisher: Medium

### Concepts and practices to ensure data quality
* Title: Concepts and practices to ensure data quality
* Date: Aug. 2022
* Author: Kevin Hu
  ([Kevin Hu on LinkedIn](https://www.linkedin.com/in/kevinzenghu/),
   [Kevin Hu on Medium](https://kevinzenghu.medium.com/))
* Link to the article:
  https://towardsdatascience.com/concepts-and-practices-to-ensure-data-quality-f3f0a95acbbf
* Publisher: Medium

### Stop Firefighting Data Quality Issues
* Title: Stop Firefighting Data Quality Issues, a quick guide to creating
  a competitive data quality assessment
* Date: Oct. 2021
* Author: Thuwarakesh Murallie
  ([Thuwarakesh Murallie on LinkedIn](https://www.linkedin.com/in/thuwarakesh/),
   [Thuwarakesh Murallie on Medium](https://thuwarakesh.medium.com/))
* Link to the article:
  https://towardsdatascience.com/stop-firefighting-data-quality-issues-4c064bcbbb53
* Publisher: Medium

### The four pillars of data observability
* Title: The four pillars of data observability
* Date: Oct. 2021
* Author: Kevin Hu
  ([Kevin Hu on LinkedIn](https://www.linkedin.com/in/kevinzenghu/),
   [Kevin Hu on Medium](https://kevinzenghu.medium.com/))
* Link to the article:
  https://towardsdatascience.com/the-four-pillars-of-data-observability-95a96a1a24e7
* Publisher: Medium

### Data Quality Validation for Python Dataframes
* Title: Data Quality Validation for Python Dataframes
* Date: Oct. 2021
* Author: Miguel Cabrera
  ([Miguel Cabrera on LinkedIn]())
* Link to the article:
  http://mfcabrera.com/blog/pandas-dataa-validation-machine-learning.html
* Publisher: [Miguel Cabrera's blog](http://mfcabrera.com/)

# Frameworks and tools

## Deequ
* GitHub page for Scala Spark version: https://github.com/awslabs/deequ
* GitHub page for the Python/PySpark version:
  https://github.com/awslabs/python-deequ

Deequ's purpose is to "unit-test" data to find errors early, before the data
gets fed to consuming systems or machine learning algorithms.

Deequ works on tabular data, _e.g._, Parquet and CSV files, database tables,
logs, flattened JSON files, basically anything that you can fit into a Spark
dataframe.

## Great Expectations (GX)
* Home page: https://greatexpectations.io/
* GitHub page: https://github.com/great-expectations/great_expectations

Great Expectations (GX) helps data teams eliminate pipeline debt, through data testing,
documentation, and profiling.

## Data Diff
* Home page: https://docs.datafold.com/development_testing/open_source
* GitHub page: https://github.com/datafold/data-diff

See how every change to dbt code affects the data produced in the modified model and downstream.

## Elementary
* Home page: https://www.elementary-data.com/

Monitor your data warehouse in minutes directly from dbt.
An analytics engineer first solution for monitoring data quality and operations

## SODA
* GitHub page: https://github.com/sodadata/soda-core
* Documentation: https://docs.soda.io/
* SODA SQL: https://docs.soda.io/soda/quick-start-soda-sql.html
* SODA Spark: https://github.com/sodadata/soda-spark
* SODA Spark is an extension of SODA SQL that allows to run SODA SQL
  functionality programmatically on a Spark data frame.

Soda SQL is an open-source command-line (CLI) tool. It uses user-defined
input to prepare SQL queries that run tests on tables in a data warehouse
to find invalid, missing, or unexpected data. When tests fail,
they surface "bad" data that you can fix to ensure that downstream
analysts are using "good" data to make decisions.

## Pydantic
* Pydantic official documentation: https://pydantic-docs.helpmanual.io/
* 8 reasons to start using Pydantic, Medium, Oct. 2021:
  https://towardsdatascience.com/8-reasons-to-start-using-pydantic-to-improve-data-parsing-and-validation-4f437eae7678

