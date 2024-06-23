# Text to SQL Conversion Project

This project demonstrates two different approaches for converting natural language queries to SQL queries and executing them on a SQLite database. The first approach leverages LlamaIndex for handling multiple tables, while the second approach uses OpenAI's GPT-3.5 model and is limited to a single table using prompt engineering.

## Table of Contents
1. [Prerequistes](#prerequistes)
2. [Installation](#installation)
3.  [Fill database file](#fill-database-file)
4. [Approach 1: Single-Table Querying with simple openai](#approach-1-single-table-querying-with-openai)
5. [Approach 2: Multi-Table Querying with LlamaIndex](#approach-2-multi-table-querying-with-llamaindex)


## Prerequistes
Add you openai api key in env file.

I have uploaded "company.db" file with data init. In whole repo i have used database path as it is in same directory. S0 make sure to add db file in same directory if you add another one




## Installation

Ensure you have Python 3.7 or higher installed. Then, clone the repository and install the necessary dependencies which are usually on first cell:

```bash
git clone git@github.com:Musab2004/text-to-sql.git
cd text-to-sql
```
## Fill-Database-File

This file is just for adding data and creating tables in the database "company.db". It is not necessary to add into db file because i have actually added this data into it. if still there is issue you can make new db file and add data into it using this script. Make sure database file name is "company.db"

## Approach-1-Single-Table-Querying-With-openai
This approach can only deal with queries for only one table employees from database. It uses only gpt prompt engineering for converting natural language into sql.

It's gradio app just run all cells and app link will be displayed in last cell


## Approach-2-Multi-Table-Querying-With-Llamaindex
This approach is using sql agents of Llama-index which can query more than one table at once.

It is also gradio app run all cells  link will appear in last cell. Make sure you have database created name "company.db"