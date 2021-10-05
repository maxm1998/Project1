# Project1

<<<<<<< HEAD


<br>
=======
# Part 1 Introduction and Data

Looking at covid, financial and health data to find out how Covid-19 has impacted the world and to find any correlations between different variables.

Data sources:
Google Finance: google sheets for stock, index, fx data
John Hopkins: Covid Data
IMF: GDP data
Kaggle: Commodity prices

What we did with the data:
Concatenating and grouping data into groups, such as fx sectors, indices, countries and dealing with a lot of date data types, using Pandas functions such as groupby...
Used Pycountry (API with list of country names and data) to check our dataframes and validate country names
Covid data from different countries can be unreliable (for example Laos only has 40 cases)  so a way to filter out outliers is to only look at countries within a certain range 
of some variable such as fatality_rate
>>>>>>> e89dd7808e9377dc56294a037f0f0e04706825db

## **Part 1 Introduction and Data:**

<br>

## What were the questions you were asking?

<br> 

**Are there any correlation between GDP per country vs the covid case numbers?**

**What are the correlation between GDP per capita vs vaccination rates of COVID 19?**

**Are there countries that are the opposite to the above? List them and their metrics?**

**Assumption is made that the higher the population density, the higher the number of cases, does the data reflect this assumption?**

**Do the richer (gdp_per_capita) countries have lower cases assuming that people are more aware of the consequences of COVID 19?**


<br>

## **Data sources:**

<br>


**Google Finance:** 
google sheets for stock, index, fx data

**John Hopkins:** 
Covid Data - available via github

**Kaggle:** 
Commodity prices

**IMF:** 
GDP data

## **Data Wrangling (How did you Clean the data?):**

**Pycountry api:** 
check dataframes and validate country names

**Cleaning dates:** 
<ol><li>Across different data sets from different sources, there were inconsistent date types such as some with timestamps, some starting with the month and some starting with year. We had to use date functions to homogenize the date types in one format.</li>
<li>Given most metrics do have the same denominator, the percentage change between each day as a standard unit of measure.</li>
</ol>

**Wrangling data:** 
<ol> <li>Concatenating data into groups, fx sectors and indices, and splicing dates</li>
<li>Using fatlity rate to narrow the covid data to reduce the noise the data set</li>
<li>Given the daily changes in prices and it would only make sense to obtain the </li>
<li>In some metrics, the number of covid cases were ever increasing and didn't represent a good measure when comparing to prices which are bidirectional. In this case, we decided to use the COVID reproduction rate to give a bidirectional view of the metric.</li>
</ol>

<br>

## **How we did it?**

<br>

<ol>
<li>Using Pandas to cut up the different dataframes and combining them to produce a meaningful data set for plotting.</li>
<li>Using Pandas functions to calculate the percentage changes and correlations readying for plots</li>
<li>Using Plotly to plot our graphs to find the correlations</li>

</ol>

<br>

## **Conclusions (What did we learn?):**

<br>

<ol><li>COVID-19 cause one of the largest falls on major indices and prices and also took the quickest time to recover those losses.
</li>
<li>Well established and economically sound countries are not well prepared for such an even on COVID-19. The way they 'weathered' these events by going into debt such as the Debt to GDP of the USA. </li>
<li>Higher life expectancy leads to higher death rate, as the numbers suggests COVID-19 kills the elderly and that living longer means you're almost likely to die from such virus given your age. </li>
<li>According to our chart, the higher the GDP per Capita suggests a higher vaccination rate. Meaning that the rich countries have a better access to the vaccines than the poorer countries. A suprising finding is that the lower the GDP per Capita, the higher the reproduction rate of the COVID19 virus.</li>
<li>Assumption was that higher the population density the higher the number of COVID cases, this was not always to be the case according to the data. It suggests that there is a weak correlation between Population Density and COVID cases which indicates there are other factors that contributes to this finding such as the measures deploy to combat the virus such as lockdowns and travel restrictions.
</ol>


