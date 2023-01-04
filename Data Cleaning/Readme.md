

There are sevral ways to handel missing data, we can either drop them, or try fill the data using our data intuitio. First we have to count how many missing rows are there, and what's the percentage of these null values. 


### Sql approach 

We can import sql library in pandas. <br>


The !pip install pandasql command installs the pandasql library, which allows you to use SQL-like syntax to query pandas dataframes.

                  #installing panda's sql library 
                  !pip install pandasql




                  #importing panda's sql library 
                  from pandasql import sqldf
                  #define a landa function for pandas' dataframe
                  pysqldf = lambda q: sqldf(q, globals())

                  #import sql 
                  query = '''SELECT * FROM sf_permits WHERE 'NULL' IS NULL'''
                  # set python sql dataframe to query
                  result = pysqldf(query)
                  #print the sql query
                  result

### Pandas' approach
