# duckdb-nodejs

Quick Start

POC - The following will seed a persistent duckdb database called db/master.duckdb with 311 request data for 2023 from data.lacity.org and output the result of `SELECT srnumber FROM requests limit 1` to the console. 

Perform the following steps from the terminal:
* git clone git@github.com:edwinjue/duckdb-nodejs.git
* cd duckdb-nodejs
* mkdir data
* mkdir db
* curl -o data/requests.csv -O https://data.lacity.org/api/views/4a4x-mna2/rows.csv?accessType=DOWNLOAD
* npm i
* node index.js
