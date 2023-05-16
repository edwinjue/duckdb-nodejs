# duckdb-nodejs

A simple "Hello World" to get started with duckdb for nodejs. 

# Quick Start
The following will seed a persistent duckdb database called `db/master.duckdb` with Los Angeles 311 service request data for 2023 using a CSV file downloaded from [data.lacity.org](https://data.lacity.org/City-Infrastructure-Service-Requests/MyLA311-Service-Request-Data-2023/4a4x-mna2) and demonstrates how to output the result of the SQL query `SELECT * FROM requests limit 1` to the console. 

Perform the following steps from the terminal:
* git clone git@github.com:edwinjue/duckdb-nodejs.git
* cd duckdb-nodejs
* mkdir data
* mkdir db
* curl -o data/requests.csv -O https://data.lacity.org/api/views/4a4x-mna2/rows.csv?accessType=DOWNLOAD
* npm i
* node [index.js](https://github.com/edwinjue/duckdb-nodejs/blob/main/index.js)

Note: Once `db/master.duckdb` has been created, you can query it immediately by loading it with `const db = new duckdb.Database('./db/master.duckdb')` and perform SQL queries using duckdb `db.*` methods. 

For more info refer to the [API documentation](https://duckdb.org/docs/api/nodejs/overview.html).
