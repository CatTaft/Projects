# Environmental & Social Factors of Industrialization from 1990-2019.
## by Catherine Taft


## Dataset

As someone who is a resident of two countries in different stages of economic development (US and Panama), and as someone with a strong interest in sustainable development, climate change, and related issues, I immediately thought to do something along the lines of development for this project. My initial interest was CO2 emissions levels, but I expanded my dataset to also include child mortality rates, GDP per capita, life expectancy and population density. These are all factors known to be influenced positively or negatively by the industrial and economic development of countries, and I wanted to examine any relationships between these to look deeper at the positive and negative impacts of development. 

The datasets I combined are:

1. CO2 Emissions (Source: Kaggle via World Bank)
2. Child Mortality; 0-5 Year Olds Dying per 1000 Born (Source: Gapminder)
3. Income Per Person/GDP Per Capita; Inflation-Adjusted (Source: Gapminder)
4. Life Expectancy in Years (Source: Gapminder)
5. Population Density per Square Km (Source: Gapminder)

The dataset had each of the above as a column (all quantitative) and all 180 countries were represented by one of the following geographic regions: North America, Latin America & Caribbean, Europe & Central Asia, Sub-Saharan Africa, East Asia & Pacific, and South Asia. My goal then was to examine each of these factors of development and their relationships to one another.

I did most of the data cleaning in Excel due to the small size of the source datasets (around 200 rows each before the required melts). I standardized numerical formats (some had for example 31k instead of 31000) and trimmed the data to the same range of years and the same countries. Here I will performed melts, renamed a few things, and combined them into a final single dataframe.


## Summary of Findings

1. Univariate - In the Univariate section I began by doing two pie charts, showing the proportion of carbon emissions in each region in 2009 and then 2019 to look at the changes between these years. We saw that the US and Europe had decreases while the rest of the world had increases. After that I did some bar charts showing mostly the 1990 values for the primary quantitative variables. Nothing was particularly surprising here if you take into account the way the data is segmented (North America for example only includes the US and Canada, not Mexico, the Caribbean or Central America).

2. Bivariate - Here I started out by looking at emissions over time for all regions and then specifically the US and China. The line chart for emissions over time showed a mix of increases and decreases of various degrees. The chart for the US and China showed the US increasing then sharply decreasing while China sharply increased and then leveled off, with the US's end rate being about double that of China's. 

I also created some paired bar charts to look at changes for different variables between 2009 and 2019. The paired bar charts were not surprising in their overall results as much as the degrees of some of the changes that took place, i.e. an absolutely enormous drop in child mortality. Then I created scatterplots. First a pairplot for all the variables, then to look at relationships between some specific variables, i.e. life expectancy and GDP. Here there were some unexpected results, for example no real relationship between population density and life expectancy, and a kind of odd plot of child mortality against GDP. 

Lastly I did two violin plots for GDP in each region, one of them showing every year in each region, each region as its own cluster, and one showing only 1990 and 2019 per region. Both of them demonstrated in different ways that wealth inequality is vastly increasing, as the median incomes in most cases remained the same or dropped, while the third quartile and max values increased drastically. The second plot showed much less clustering around the mean. It was discouraging information but that is my favorite pair of plots from the whole project.

3. Multivariate - This final section was a bit brief since I spent the bulk of my time in bivariate, but here I did two scatterplots looking at three regions of interest (the Middle East, Europe & Central Asia, and East Asia & Pacific), with each region separated by color, and in each plot I chose a third variable to be depicted by size. In the first it was life expectancy, and in the second it was population density. The firstplot showed an increase in life expectancy as GDP increases, and GDP seemed to be more of an indicator than emissions, although we had previously seen some correlation between emissions and GDP. The second plot demonstrated that population density increased towards the upper end of each region's emissions and GDP, which indicates an urbanization as countries develop. Then I did a scatterplot of emissions and GDP using a color bar to represent child mortality rate, which was one of the variables that hadn't made much sense earlier. This showed a much clearer relationship, with high mortality rates at both low GDP and low emissions, decreasing along both axes as GDP and emissions increase.


## Key Insights for Presentation

1. The change in emissions really depends on development status. The wealthier countries (US, Canada, Europe) are in a position to start exploring alternative sources of energy or carbon cap and trade, and reducing emissions. Developing countries do not have this luxury, so while we see a decrease in the INCREASE of emissions, overall they're still increasing.

2. Since emissions increases, while being horrible for the environment, are still a metric of economic growth, we also see life expectancy increase and child mortality rates decrease significantly. GDP is positively correlated with this as well as emissions rates.

3. Wealth inequality has increased to a staggering degree, so the positive economic developments we see in aggregate in the previous examples do not translate uniformly across society.