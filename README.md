# School_District_Analysis

## Overview of Project
The goal of this project is to analyze a raw dataset containing student test scores from various schools within a school district. The user of the final reports would like to see some key metrics on what affected student testing performance and then to use that information to make decisions on future funding awards within the district.

### Purpose
Explore the Python Pandas library, learning to use the library to read data from a file and create meaningful data visuals for analysis. Specifically learn how to create DataFrames, how to manipulate them to contain useful information, and how to build off of DataFrames to build summary reports containing key metrics.

## Analysis and Challenges

### Analysis of PyCitySchools Module Activity
There are a number of useful reports initially created from the guided module activity, including a distict summary table and associated tables to narrow down on specific variables that may have contributed to student success or lack thereof in the district testing.

<p align="center">
  <img src="https://github.com/cb19weber/School_District_Analysis/blob/main/Resources/top_five_original.png" />
</p>

The initial analysis of the entire dataset revealed the top five performing schools in the district. We are then left to ponder, what exactly separated these schools from the pack? There is a significant amount of data present even in the above <i>summary</i> table. A common assumption might be that the schools with the highst levels of funding result in the greatest student success.

<p align="center">
  <img src="https://github.com/cb19weber/School_District_Analysis/blob/main/Resources/spending_summary_original.png" />
</p>

Many might be surprised to see the data point out a linear relationship that actually shows the opposite of this common assumption. While the relatively clear relationship demonstrated in the data here likely does not suggest that spending <i>less</i> on educational funding is the answer, it does demonstrate that funding and student testing results more likely are correlated than having a causal relationship.

While a seemingly striking dichotomy between charter and district schools was exhibited, probably the most insightful information came from the relationship between school size and student success.

<p align="center">
  <img src="https://github.com/cb19weber/School_District_Analysis/blob/main/Resources/size_summary_original.png" />
</p>

While it may have seemed that charter schools held a clear advantage, the truth is more likely revealed in school size. In fact the largest charter school was home to only 2,283 students; conversely the <i>smallest</i> district school had to make room for 2,739 students. Multiple district schools in the dataset are home to between four and five thousand students. The revelation is so impactful that a reader is forced to ponder whether increasing funding per school might be inferior to just building more schools.

### Analysis of PyCitySchools Challenge
The challenge offered some very intriguing nuance to the weekly project. One grade level at one of the schools was found to have manipulated testing data. The extent of the dishonesty was unknown, so the decision was made to eliminate that particular sliver of data from the analysis. There were multiple challenges in doing this.

The data was still read from the original files, but once the DataFrames were created in jupyter notebook, the affected data had to be altered so as not to negatively impact analysis. This required isolated the data in the DataFrame and replacing values using the NumPy library with NaNs. The analysis then had to be repeated, and percentage calculations adjusted based on a different sample size. The class and school of students remained in the overall summary, but their test scores were removed. This left the dataset whole, but removed data that unfairly altered the analysis.

### Challenges and Difficulties Encountered
There is <i>so much to learn</i> with the pandas library! This was a huge module and required a lot of getting into the documentation to understand the syntax of various functions and methods. I definitely feel like I'm on a steep learning curve, but I also feel like the experience is going to make a big difference. Being able to dig into data and build various tables to analyze, visualize, and understand it is an incredible tool.

I think my biggest challenge this week was time management with my professional obligations. But I am proud of my effort and the outcome of the work here. I am excited to continue learning pandas and implement it further in my career.

## Results
Being able to create version specific environments within Anaconda, utilizing the Pandas library, reading data from csv or excel files, merging datasets and performing analysis has already given me some great ideas of how to apply this in my current role. I believe I can take the same tools I've learned in this module to create a great deal of automation in revenue recognition. My goal is to build DataFrames out of raw data from the ERP, merge and analyze the data to get a complete picture, and be able to author custom reports that can provide the executive committee with the best possible, most accurate information in order to make decisions that will help drive our company to great success.