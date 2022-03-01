# Reading Multiple Files into a Single Dataframe

Occassionally, the data that is needed for some anatlytics task is held in several files. Many times, this means that the data needs to be read into a single dataframe for effective analysis. One way to acheive this is to read each of the files into a respective dataframe; then at the end, combine all the dataframes into a single dataframe. While this works, it requires the use of several read statements (as many as there are files); which is not very convenient if there are alot of files to be read e.g. thousands of files. Another problem with this approach is that the name of each of the files needs to be explicitly specified; again not a very convenient thing to do, if we are dealing with several files.

This xxx describes an approach for reading multiple files into a common directory without having to explicitly write several `read` statements and specify the name of each file. A caveat to this is that; it assumes that all the files are in the same location (folder) and have a similar structure.

We will use an openly sourced dataset, the US Social Security Baby Name catalog https://www.ssa/gov/oact/babynames to demonstrate this. This catalog records the names given to babies born since the year 1880. The data can be downloaded through the link https://www.ssa.gov/oact/babynames/limits.html
