# Genetic-Structure-Tools
R Functions for plotting and working with STRUCTURE files

<img src="https://static1.squarespace.com/static/54ad6922e4b0ab38fefa18b1/t/57323b9a27d4bdb26406fc50/1462909877175/K%3D4+Plot?format=750w"> 

Here you will find a couple of functions that are useful for plotting the results of STRUCTURE in R. Just download the "STRplot.r" file and open R. Set your working directory to your Results folder from your STRUCTURE run and also put your .txt formated STRUCTURE infile in this directory. You can then run Source("STRplot.r") and you will now be able to run the two functions you need. 

## Getting Started
* If you are running this on your own data you are now ready to go. If not, I have provided some example files, just download these to a single directory and you should be able to work with these files

Lets start by turning the ugly STRUCTURE outfile into a clean .csv file

`>read.STR("All Glynnii.txt","No Add Inf Lamb Final_run_10_f")`

Now check your folder and you should have a file called "k4.csv", or if your running this on your own data it will be "kx.csv" where x= the k value you used. 

If this file is in the order that you would like you are all set, if not you can reorder the file any way that you would like and then save it as "Order.csv", just be sure to keep your original "k4.csv" as well.

Now you can plot with:

`>plotSTR("k4.csv")`

or if you reordered the file you will use:

`>plotSTR("k4.csv",Order.csv="Order.csv")`

This should output the above .pdf





