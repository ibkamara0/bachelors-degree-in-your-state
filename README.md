# Personal Statement
First off, I would like to say I hope this country can truly grow after the tragic death of George Floyd. I hope that whoever is reading this can understand that you may not have the same views or come from the same background as the person next to you but, everyone deserves respect. No matter your race, sexual orientation, gender, religion, etc. everyone deserves your respect, and should be treated with such. Hopefully, once we start respecting one another, we can get to the point of loving one another, and accepting our differences. Keep fighting for respect, keep fighting for love, keep fighting for everything good in this country, and hopefully we can grow as a nation.

Thank you,<br/>
Ibrahim Kamara

# Background
Now for a little background on this project. Being a recent graduate and wanted to show my passion and skills to employers, I got curious. I decided to apply some of my skills to a project that appealed to my peers and I. Given we all just got our bachelor's degrees and some of us our looking for employment. I wanted to where our bachelor's degrees most affected income and unemployment rates. Below, I get to take you along the journey of how this question was answered. Enjoy.

# Overview
- In this project data will be collected from US Department of Agriculture Economic Research Service on Unemployment, Median Household Income, and Education Attainment
- Raw data will be cleaned and manipulated for visualization and model development
- Lastly, models and visualizations will be translated and interpreted to give data meaning in context of our research question.

# Data Cleaning
- Load the excel files (education and unemployment/income data) into dataframes
- Extract from the dataframes, only the columns needed
- Rename the columns so they're easier to manipulate and interpret
- Create a function that let's you insert the state abbreviation and return a dataframe needed for this
- Below is you see the results of running the function:

  ![Area Dataframe](https://github.com/ibkamara0/bachelors-degree-in-your-state/blob/master/Dataframe.JPG)

# Exploratory Data Analysis
- Create a correlation matrix to show the correlation between the variables
- Represent the correlation matrix in a heatmap (this was done for fun!). Below you can see an explanation and visual representation of the heatmap for New York
  - With correlation shows how variables are related on a scale of -1 to 1:
    - **1 = Positive correlation (light red):**  indicating a perfect positive correlation meaning as one variable increase so does the other. 
    - **-1 = Negative correlationn (light blue):** meaning the opposite as one increases the other variable decreases. 
    - **0 = No correlation (black):**  Meaning that the two variable have no relationship
    
    ![heatmap](https://github.com/ibkamara0/bachelors-degree-in-your-state/blob/master/heatmap.JPG)
 - We can see correlation between Percentage of People with Bachelor's Degrees by Area vs. Unemployment or Median Household Income measured and visualized in the heatmap. We can see that New York, has a positive correlation for Percentage of People with Bachelor's Degreess by Area vs. Median Household Income. This means in the state of New York the higher the percent of people with a bachelor's degrees in an area the higher the median household income
- Now, we pull the correlation metrics that we want for each state by creating a function that iterates through each state abbreviation and returns a dataframe with the state, correlation between Bachelor's Degrees by Area (%) vs Unemployment Rate 2018, and Bachelor's Degrees by Area (%) vs. Median Household Income 2018.
Example of what was done is see below

   ![state dataframe](https://github.com/ibkamara0/bachelors-degree-in-your-state/blob/master/State%20Dataframe.JPG)
   
# Results
- Now we're ready to visualize the results
- A choropleth map was created to display the correlation between Percentage of People with Bachelor's Degree vs Unemployment Rate and Median Household Income of each state
- Below is a representation of which states have the highest correlation between Bachelor's Degrees (%) and Median Household Income. In this the darker states have a correlation metric close to 1, while the lighter states have a metric close to -1. 
  ![income choropleth map](https://github.com/ibkamara0/bachelors-degree-in-your-state/blob/master/IncomeMap.JPG)
- This means that if we take a state like California with high correlation we can see how the percentage of people with bachelor's degrees affects the median household income in the state.(Seen below)
![california correlation](https://github.com/ibkamara0/bachelors-degree-in-your-state/blob/master/CaliIncome.png)
- Let's do the same with the Bachelor's Degrees (%) vs. Unemployment Rate. Again, darker colored states have correlation close to 1, while lighter colors are closer to -1. You can see California as having a negative correlation between the two variables because of how light it is.
![unemployment choropleth map](https://github.com/ibkamara0/bachelors-degree-in-your-state/blob/master/unemploymentMap.JPG)
- Again, looking at california you see how percentage of people with bachelor's degrees affects the unemployment rate in that state.  (Seen below)
![california correlation](https://github.com/ibkamara0/bachelors-degree-in-your-state/blob/master/CaliUnemployment.png)

# Conclusion
Based on this project you can see that Bachelor's Degrees affect the Unemployment Rate and the Median Household Income in certain states. Interpreting this further, you can see which states have competive incomes based on your education level, and the states where you may find more job opportunities with your education.

# Closing Remarks
This is a project done for fun and experience. Feel free to reach out to me at ibkamara1997@gmail.com or message me on [LinkedIn](https://www.linkedin.com/in/ibrahim-kamara-81b427139/). I would love to hear your feedback as I continue to strengthen my portfolio (good or bad). Also, I'm on the hunt for entry level positions, I'd love to have a conversation about that as well. Continue to spread love.

Thank you for reading,<br/>
Ibrahim Kamara

# Resources and Code
- **Link to dataset:** https://www.ers.usda.gov/data-products/county-level-data-sets/download-data/
- **Link to my jupyter notebook:** https://github.com/ibkamara0/bachelors-degree-in-your-state/blob/master/Data%20Cleaning.ipynb
- **United State GeoJSON file:** https://github.com/python-visualization/folium/blob/master/tests/us-states.json
