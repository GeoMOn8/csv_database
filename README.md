
# CSV_to_database

This script will automatically import CSV files to your postgres/postgis database. Just place the CSV files in the same directory as the notebook and run the notebook. The notebook will automatically clean the file name and column headers, create the db table, and copy the file over to the database. The table names are the same names as the file names. However, all upper case characters are changed to lower case, spaces are converted to underscores, and all symbols are removed.

* Main goal = load data from CSV into a postgres/postgis database
* Who will use this? Me and colleges 
* What problem does this software solve? creating space on hardrive additional place of storage(security)




## What I would like to add later

* Dockerize it for easy deployment
* Have a basic UI where there is a password and to choose from a list of exsisting databases or create a new database that will connect to postgis.

## Worth mentioning

I used SQL to convert double-pricision data-type to GEOM data-type in the Lat-lon columns.

## Requirements

* anaconda needs to be installed
* docker needs to be installed to install Jupyter notebook
* psycopg2 needs to be installed
* mysql connector needs to be installed
