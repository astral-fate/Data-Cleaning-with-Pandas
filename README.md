# Data-Cleaning-with-Pandas





## Table of content

1. [Handling Missing Values](#Handling-Missing-Values)
2. [Scaling and Normalization](#Scaling-and-Normalization)
3. [Parsing Dates](#Parsing-Dates)
4. [Character Encodings](#Character-Encodings)
5. [Inconsistent Data Entry](#Inconsistent-Data-Entry)





# Handling Missing Values

There are sevral ways to handel missing data, we can either drop them, or try fill the data using our data intuitio. First we have to count how many missing rows are there, and what's the percentage of these null values. 


### Sql approach 

We can import sql library in pandas

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


# Scaling and Normalization

# Parsing Dates

# Character Encodings

# Inconsistent Data Entry

