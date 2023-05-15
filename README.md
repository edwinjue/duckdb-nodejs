# duckdb-nodejs

A simple "Hello World" program to get started with using duckdb for nodejs. 

# Quick Start
The following will seed a persistent duckdb database called `db/master.duckdb` with 311 request data for 2023 using a CSV file downloaded from data.lacity.org and output the result of a sample SQL query `SELECT srnumber FROM requests limit 1` to the console. 

Perform the following steps from the terminal:
* git clone git@github.com:edwinjue/duckdb-nodejs.git
* cd duckdb-nodejs
* mkdir data
* mkdir db
* curl -o data/requests.csv -O https://data.lacity.org/api/views/4a4x-mna2/rows.csv?accessType=DOWNLOAD
* npm i
* node index.js

Note: Once `db/master.duckdb` has been created, you can query it immediately by loading it with `const db = new duckdb.Database('./db/master.duckdb')` and perform SQL queries using duckdb `db.*` methods. 

For more info refer to the [API documentation](https://duckdb.org/docs/api/nodejs/overview.html).
