# Final-Project-Tableau

## Project/Goals
The goal of this project is to demonstrate Tableau skills to visualize data and help draw meaningful insights for a company. 

## Process
### Step 1: Connect to Data
A dataset containing FIFA18 player ratings and market values was provided. Connected the csv file through tableau and then proceeded to review datatypes.  
### Step 2: Detect different data types and identify missing datatypes. 
The dataset consisted of two main datatypes: Integers for rating related categories (positional/attributes/market values) and strings for other categories such as (names,nationalities,clubs,etc). Nationalaties needed to be changed to included a geographic - country. A key missing field was dates that would've been useful to analyze time related data and make projections. 
### Step 3: Build visualizations to learn more about the dataset.
Two main types of visualizations were created. 
1. Market Level  
2. Club Level (players at one club)   
### Step 4: Identify important features about the dataset (why) and establish a use case. 
On a market level, the key features that helped to identify which clubs are the top competitors are Value and Wages. The total value of the players a club help reflect the quality of the players that are at the team without being negatively impacted by low rated youth players (i.e if using a club's average rating, low rated players would lower the team's average). The total wages for team helps to reflect the overall budget that a team can afford and as result help attract top ranked players.

On an individual club level, the players overall rating is the most important feature because this is a rating meant to reflect how well a player ranks for thier position on a scale of 0-99. Individual attributes such as short passing and sprint speed are also relevant when comparing players, however similar attributes should be grouped into their main categories such as pace, shooting, dribbling, passing, defending, and physicality. The trends found in the data indicated that midfielders generally have good passing and dribbling, attackers have good shooting and dribbling, and defenders have good physicality and defending. These main attributes should be used for comparing indivual players based on their positions.  

After creating the visualizations, I wanted to use the data to identify which youth players should Manchester City use as totational players for the first team. 


## Results
Using project option 2 (FIFA 18 Dataset), I wanted to address "Which youth players should Manchester City use as rotational players for the first team based on their potential, and which first team player roles could they fill in for?"  

The following visualizations were created: 

Market Level
1. Club Value vs Wages Scatter Plot.
Using a parameter filter on Total Player Values of 100,000,000 euros and clusters of 4. Cluster 4 includes the best of Europe, Cluster 3 shows league winners, Cluster 2 shows top 4 contenders, and Cluster 1 shows top 10 contenders. 

This type of visual was chosen because it helps group top flight clubs of europe (first by filtering with the parameter) and the clusters give a sense of what other clubs are at a similar level on a financial level.    

2. Top Players Map
The map plots a calculated field of player counts, using a filter parameter based on overall rating. An overall rating of 85 was used to set "Top Rated" players because of the scale of 0-99 in place for the field with 94 being the highest rated player. This map shows that the top players are coming from South America or Europe.  

3. Top Players Bar Plot
This visualization was used because it builds on the previous map to understand how many players fall into a rating. The scarcity of top rated players can be seen as the rating increases. 

Club Level (Manchester City)
4. Core Players - Grouped Bar
After establishing the top players in the market are 85 rated, this type of visual was chosen to filter a club for their top players and see what positions they play in and what their key attributes (calculated fields grouping stats for pace, shooting, passing, dribbling, defending, physical). 

3 midfielders, 1 striker, and 1 defender were identified. The midfielders each strong passing and dribbling stats, the striker has strong shooting and pace stats, and the centre back has strong defending and physicality stats.    

5. Potential Players - Stacked Bar
This type of visualization was selected because it allows two different statistics for an individual player to be displayed together in one bar. 
The dark lines on each bar indicate the player's potential stats, and the blue bar indicate a players current overall rating. After including age, it can be seen that as the players reach their mid 30s, they have peaked in terms of overall rating and don't have any more room to grow whereas the youngest players have the highest rooms to grow. This visual is useful when looking at a club's full squad.    

6. Youth Players - Grouped Bar 
This visual replicates the core players visual, but uses the potenial rating instead of overall to identify top prospects. The top prospects are also filtered down based on age and a calculated field that measures their room to grow (potential - overall). 
Players are colour coded based of the core player they best replicate (based on their best attributes). In conclusion the top prospects to incorporate into the first team for midfield are Phil Foden (for Kevin de Bruyne), Brahim Diaz (for David Silva) and Zinchenko (for Gundogan). The prospects for striker is Gabriel Jesus (for Sergio Aguero). The prospect for CB is Adarabioyo (for Kompany). 


Dashboard: 
The final dashboard provides an insight on individual players at Manchester City, particulary visualizations #4,5,6. A map was also included to compare where top rate players are from so if the team should look into investing further in recruiting youth from a location, they could easily determine if they have a better chance of finding a top prospect. 

## Challenges 
Challenges I faced during the project was implementing the map because of nation mismatches. To resolve this issue, I manually matched the nationaliationies with errors. 

## Future Goals
If i had more time, I would link the database to previous editions of FIFA to get yearly player data. This would allow me to do a analysis on the growth of players on an annual basis and use it to also create better projection models. 

