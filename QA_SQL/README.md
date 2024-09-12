# Build a Question/Answering system over SQL data

## Overview

The basic ways to create a Q&A chain and agent over a SQL database. These systems will allow us to ask a question about the data in a SQL database and get back a natural language answer. Agents can query the database in a loop as many time as it needs to answer the question.

## Data

We will use a dataset of a real-world database.
- File: `tables.txt` describe the tables of the database.
- File: `examples.txt` contains examples questions -> query -> answer[optional].

## Evaluation

We will use the following metrics to evaluate the performance of the system:
- File: `evaluation.txt` contains the evaluation results.

## Architecture:

At a high-level, the steps of most SQL chain and agent are:
- Convert question to SQL query: Model converts user input to a SQL query.
- Execute SQL query: Execute the SQL query
- Answer the question: Model responds to user input using the query results.

![alt text](image.png)


## Solutions:

## Development cycle:

- 