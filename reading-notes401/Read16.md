## Machine Learning
Machine learning: Machine learning is the practice of teaching computers how to learn patterns from data, often for making decisions or predictions.


First, we must clear up one of the biggest misconceptions about machine learning:

Machine learning is not about algorithms.

When you open a textbook or a university syllabus, you'll often be greeted by a grocery list of algorithms.

This has fueled the misconception that machine learning is about mastering dozens of algorithms. However, it's much more than that...

Machine learning is a comprehensive approach to solving problems...

...and individual algorithms are only one piece of the puzzle. The rest of the puzzle is how you apply them the right way.


## Terminologies
-Model - a set of patterns learned from data.

- Algorithm: a specific ML process used to train a model.
Training data: the dataset from which the algorithm learns the model.
- Test data: a new dataset for reliably evaluating model performance.
- Features: Variables (columns) in the dataset used to train the model.
- Target variable: A specific variable you're trying to predict.
Observations: Data points (rows) in the dataset.

## Exploratory Analysis


The purpose of exploratory analysis is to "get to know" the dataset. Doing so upfront will make the rest of the project much smoother, in 3 main ways:

- You’ll gain valuable hints for Data Cleaning (which can make or break your models).
- You’ll think of ideas for Feature Engineering (which can take your models from good to great).
- You’ll get a "feel" for the dataset, which will help you communicate results and deliver greater impact.

## Data Cleaning

Better data beats fancier algorithms.

In other words... garbage in gets you garbage out. Even if you forget everything else from this course, please remember this point.

In fact, if you have a properly cleaned dataset, even simple algorithms can learn impressive insights from the data!

Obviously, different types of data will require different types of cleaning. However, the systematic approach laid out in this lesson can always serve as a good starting point.

## Algorithm
algorithms are a set of instructions that are executed to get the solution to a given problem. Since algorithms are not language-specific, they can be implemented in several programming languages. No standard rules guide the writing of algorithms.

## Models

A model is a Python class that inherits from the Model class. The model class defines a new Kind of datastore entity and the properties the Kind is expected to take. The Kind name is defined by the instantiated class name that inherits from db.


## Data Wrangling

Data Wrangling is the process of gathering, collecting, and transforming Raw data into another format for better understanding, decision-making, accessing, and analysis in less time. Data Wrangling is also known as Data Munging.

## Here are the steps we’ll take for our analysis:

1. Set up your environment:  
First, make sure you have the following installed on your computer:  
Python 2.7+ or Python 3
Pandas
Jupyter Notebook (optional, but recommended)
We strongly recommend installing the Anaconda Distribution, which comes with all of those packages. Simply follow the instructions on that download page.



2. Import libraries and dataset.  
Let's start by importing Pandas, the best Python library for wrangling relational (i.e. table-format) datasets. Pandas will be doing most of the heavy lifting for this tutorial.  
**Tip**: we'll give Pandas an alias. Later, we can invoke the library with pd.  

    **Data Dictionary** (for code GWA_BTC):    
- **Date**: The day on which the index values were calculated.
- **Open**: The day's opening price index for Bitcoin in US dollars.
- **High**: The highest value for the price index for Bitcoin in US dollars that day.
- **Low**: The lowest value for the price index for Bitcoin in US dollars that day.
- **Close**: The day's closing price index for Bitcoin in US dollars.
- **Volume**: The volume of Bitcoin traded that day.
- **VWAP**: The volume weighted average price of Bitcoin traded that day.
- **TWAP**: The time-weighted average price of Bitcoin traded that day.


3. Understand the data.
One of the most common reasons to wrangle data is when there's "too much" information packed into a single table, especially when dealing with time series data.

    Generally, all observations should be equivalent in granularity and in units.  

    There will be exceptions, but for the most part, this rule of thumb can save you from many headaches.

    - **Equivalence in Granularity** - For example, you could have 10 rows of data from 10 different cryptocurrencies. However, you should not have an 11th row with average or total values from the other 10 rows. That 11th row would be an aggregation, and thus not equivalent in granularity to the other 10.  
    - **Equivalence in Units** - You could have 10 rows with prices in USD collected at different dates. However, you should not then have another 10 rows with prices quoted in EUR. Any aggregations, distributions, visualizations, or statistics would become meaningless.      
<br>

4. Filter unwanted observations.  
One of the simplest yet most useful data wrangling techniques is removing unwanted observations.

    In the previous step, we learned that GWA codes are aggregations of the regional MWA codes. Therefore, to perform our analysis, we only need to keep the global GWA codes

5. Pivot the dataset.
Next, in order to analyze our momentum trading strategy outlined above, for each cryptocurrency, we'll need calculate returns over the prior 7, 14, 21, and 28 days... for the first day of each month.

    However, it would be a huge pain to do so with the current "stacked" dataset. It would involve writing helper functions, loops, and plenty of conditional logic. Instead, we'll take a more elegant approach....

    First, we'll pivot the dataset while keeping only one price column. For this tutorial, let's keep the VWAP (volume weighted average price) column, but you could make a good case for most of them.

6. Shift the pivoted dataset.
To easily calculate returns over the prior 7, 14, 21, and 28 days, we can use Pandas's shift method.

    This function shifts the index of the dataframe by some number of periods.

7. Melt the shifted dataset.  
Now that we've calculated returns using the pivoted dataset, we're going to "unpivot" the returns. By unpivoting, or melting the data, we can later create an analytical base table (ABT) where each row contains all of the relevant information for a particular coin on a particular date.

8. Reduce-merge the melted data.  
All that's left to do is join our melted dataframes into a single analytical base table. We'll need two tools.

    The first is Pandas's merge function, which works like SQL JOIN. For example, to merge the first two melted dataframes.


9. (Optional) Aggregate with group-by.
As a final step, if we wanted to only keep the first days of each month, we can use a group-by followed by an aggregation.

    1. First, create a new 'month'  feature from the first 7 characters of the Date strings.
    2. Then, group the observations by  'Code' and by  'month'. Pandas will create "cells" of data that separate observations by Code and month.
    3. Finally, within each group, simply take the  .first() observation and reset the index.





