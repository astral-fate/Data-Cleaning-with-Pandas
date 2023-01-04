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

# Character Encodings

# Inconsistent Data Entry

