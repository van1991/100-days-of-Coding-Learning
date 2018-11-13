# 100-days-of-Coding-Learning

## Step 1: Basic Commands to access the data

#remove all the objects stored <br />
rm(list=ls())

#set current working directory <br />
setwd("D:/Analytics/Codes")

#Current working directory <br />
getwd()

#instaling packages <br />
install.packages("dplyr")

#Install multiple packages at a time <br />
install.packages(c("dplyr","plyr","reshape","ggplot2","data.table"))

## Load data in R
#reading CSV <br />
data = read.csv("MissingInfo-V2.csv", header = T) 

#reading Excel sheet <br />
library(xlsx)
data_excel = read.xlsx("MissingInfo-V2.xlsx", sheetIndex = 1)

#reading .txt file as dataframe <br />
data_text = read.delim("MissingInfo-V2.txt", sep = "\t", header = T) 

#We are considering mtcars dataset to understand R commands
data = mtcars
 
#Getting the column names of the dataset
names(data)

#Getting the structure of the dataset
str(data)

#Getting the number of variables and obervation in the datasets
dim(data)

#Getting first 10 rows of the dataset
head(data, 10)

#Getting the last 10 rows of the dataset
tail(data, 10)
