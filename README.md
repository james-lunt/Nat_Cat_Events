Analysis & Segmentation of Natural Catastrophe Events

Definition of Nat-Cat Event:
A "nat cat event" refers to a "natural catastrophe event." These are significant natural events that cause substantial damage and disruption. Examples of natural catastrophe events include:
•	Earthquakes
•	Hurricanes
•	Tornadoes
•	Floods
•	Wildfires
•	Tsunamis
•	Volcanic eruptions
These events often result in significant economic losses, property damage, and can have severe impacts on human life and the environment.

We are providing a dataset cataloguing media articles on Nat Cat events. This dataset was extracted from GDelt API.


Part 1:
Task 1:
Exploratory Data Analysis: 
o	Perform an initial inspection to understand the structure and content of the dataset. 
o	Provide a summary of the dataset, including the number of articles, the range of publication dates, and the basic structure of the data, average length of titles, missing data, etc. 


Task 2:
o	For this task, your main focus will be the analysis of the Title of the article
o	Dataset is extremely noisy – contains a lot of irrelevant titles of articles
o	General cleaning/prep should include duplicate removal, extra whitespace, special characters etc.  
o	Focus should be on actual nat cat events that have occurred. 
o	Criteria for Nat-Cat article titles we are looking for:
	They must contain a location
	They must represent an event that has occurred


Part 2:
to develop a component that utilizes the cleaned data from Part 1 to assign each type of natural catastrophe title into its corresponding category. The result should consist of 5 groups, specifically Earthquake, Floods, Volcano, Tornado, and Wildfire