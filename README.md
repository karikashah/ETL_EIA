# Data Sources
•	CSV files located on EIA.gov
•	Web API located on EIA.gov

# Detailing the process of the extraction, transformation, and loading steps
•	Read the CSV file & created Dataframe for Summary (Net generation of Fuel types from All US States)
•	Read API statewise for each fuel type – for this project I have used 6 fuel types:
o	Non-renewable – Coal, Nuclear & Natural Gas
o	Renewable – Wind, Hydroelectric, Solar
•	Transformed the API results to extract Year & fuel type generation
•	Load into Mongo DB – created Mongo connection. For each state, inserted first fuel type & then updated each time the same document to insert columns for that particular state & year.

# Hypothesis: 
That green energy revolution and oil prices as high as 150 $/barrel has driven innovation and shifted the electricity production sources. 

Analyze: Price structure of electricity based on the production source. 
Assumption: Electricity production = electricity consumption. 

Objective:
1.	Green revolution in electricity field
2.	Observe trend statewise to see renewable energy production vs non-renewable
3.	Identify top 3 states adopting renewable energy
4.	Identify top green energy

Resources: 
•	https://www.eia.gov/electricity/
•	https://www.eia.gov/beta/electricity/data/browser/
