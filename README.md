# Data-Cleaning-with-Pandas





## Table of content

1. [Handling Missing Values](#Handling-Missing-Values)
2. [Scaling and Normalization](#Scaling-and-Normalization)
3. [Parsing Dates](#Parsing-Dates)
4. [Character Encodings](#Character-Encodings)
5. [Inconsistent Data Entry](#Inconsistent-Data-Entry)





# Handling Missing Values
The procces of cleaning data: <br>
1. read cvs file
2. show the head() of the data
3. use isnull() pandas' function to see the number of null rows in the dataset
4. count the total of null value using sum() functuin
5. find the shape of this dataset (rows & colms)
6. find the product of the data; meaning rows*columns, <br>
which you can do uding numpy function product; data_cells = np.product(mydata.shape)
7. find the percentage of these missing data; percetage = ((total_of_missing_values)/(data_cells))*100
8. use your data intution to know why these values were missing; not recorded or don't exixit. 
9. if the missing vlues are 80% and above we will delete the row or the column
10. we can fill the null values with mean, median, mode or 0 or any other values


# Scaling and Normalization

# Parsing Dates

Steps to prase the dates:
1. find the data types
2. display the column 
3. check the length of the date 
4. manually modify the dates if they are entired in inncorrect way using .loc
5. cast the data type from object to the specfic format such as <b> format="%m/%d/%Y" </b>
6. Visualze the data to double check. Use the seaborn library as: sns.distplot(column, kde=False, bins=31)


we have to first check the type of the column as follows:

      mydataframe['mycolumn'].dtype

dtype is a short cut for data type.


then show a portion of the data to check:

        mydataframe[300:400]
        
we then see the length of these indeses:

        date_lengths = earthquakes.Date.str.len()
        date_lengths.value_counts()


# Character Encodings

# Inconsistent Data Entry

