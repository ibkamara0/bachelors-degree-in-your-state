# Personal Statement
I would like to say I hope this country can truly grow after the tragic death of George Floyd. I hope that whoever is reading this can understand that you may not have the same views as the person next to you but everyone deserves respect. No matter your race, sexual orientation, gender, religion, etc. everyone deserves your respect, and shouldn't be treated as if they don't. Hopefully, once we start respecting one another, we can get to the point of loving one another, and accepting our differences. Keep fighting for respect, keep fighting for love, keep fighting for everything good in this country, and hopefully we can grow as a nation.

Thank you,
Ibrahim Kamara

# Background
Being a recent graduate, I simply was curious. I decided to apply some of my skills to a project that applied to my peers and I. I wanted to see does your degree really have an effect on your income, or whether you get a job? We'll let's see!

# Overview
- In this project data will be collected from US Department of Agriculture Economic Research Service on Unemployment, Median Household Income, and Education Attainment
- Raw data will be cleaned and manipulated for visualization and model development
- Lastly, models and visualizations will be translated and interpreted to give data meaning in context of our research question.

# Data Cleaning
- Load the excel files (education and unemployment/income data) into dataframes
- Extract from the dataframes only the columns needed
- Rename the columns so they're easier to manipulate and interpret
- Create a function that let's you insert the state abbreviation and return a dataframe needed for this
- Below is you see exactly what was done:

  ![Area Dataframe](https://github.com/ibkamara0/bachelors-degree-in-your-state/blob/master/Dataframe.JPG)

# Exploratory Data Analysis
- Create a correlation matrix to show the correlation between the varialbles
- Represent the correlation matrix in a heatmap (this was done for fun!). Below you can see and explanation and visual representation of the heatmap for New York
  - With correlation shows how variables are related on a scale of -1 to 1:
    - **1 = Positive correlation:**  indicating a perfect positive correlation meaning as one variable increase so does the other. 
    - **-1 = Negative correlation:** meaning the opposite as one increases the other variable decreases. 
    - **0 = No correlation:**  Meaning that the two variable have no relationship
    
    ![heatmap](https://github.com/ibkamara0/bachelors-degree-in-your-state/blob/master/heatmap.JPG)
 - We can see correlation between people with a bachlor's degree(%) and unemployment or median household income measured and visualized in the heatmap. We can see that New York has a positive correlation for percentage of people with bachelor's degrees in an area and median household income. This means in the state of new york the higher the percent of people in an area contribute to a higher median household income
- Now, we pull the correlation metrics that we want for each state by creating that iterates through each state abbreviation and returns a dataframe with the state, correlation between bachelor's degree (%) vs Unemployment Rate 2018, and bachelor's degree (%) vs. Median Household Income 2018.
Example of what was done is see below

   ![state dataframe](https://github.com/ibkamara0/bachelors-degree-in-your-state/blob/master/State%20Dataframe.JPG)
   
# Results
- Now we're ready to visualize the results
- A choropleth map was created to display the correlation between bachelor's degree vs unemployment and median household income of each state
- Below is a representation of which states have the highest correlation between bachelor's degree(%) and median household income. 
  ![income choropleth map](https://github.com/ibkamara0/bachelors-degree-in-your-state/blob/master/IncomeMap.JPG)
- This means that if we take a state like california with high correlation we can visually see how the percentage of people with bachelor's degree affects the median household income.(Seen below)
![california correlation](https://github.com/ibkamara0/bachelors-degree-in-your-state/blob/master/CaliIncome.png)
- Let's do the same with the unemployment rate
![unemployment choropleth map](https://github.com/ibkamara0/bachelors-degree-in-your-state/blob/master/unemploymentMap.JPG)
- Again, looking at california you see how percentage of people with bachelor's degrees affect the unemployment rate in that state. (Seen below)
![california correlation](https://github.com/ibkamara0/bachelors-degree-in-your-state/blob/master/CaliUnemployment.png)

# Conclusion
- Based on the research it can be said that having a bachelor's degree can have an affect on the unemployment rate and median household income, but only in certain states.

# Resources and Code
- **Link to dataset:** https://www.ers.usda.gov/data-products/county-level-data-sets/download-data/
- **Link to my jupyter notebook:** https://github.com/ibkamara0/bachelors-degree-in-your-state/blob/master/Data%20Cleaning.ipynb
- **United State GeoJSON file:** https://github.com/python-visualization/folium/blob/master/tests/us-states.json
