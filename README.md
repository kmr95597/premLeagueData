# premLeagueData

## Group Name:
29704 Group 9

## Team Members:
Kevin Reilly [@kmr95597](https://www.github.com/kmr95597),
Alex Tran [@alexandretran1](https://www.github.com/alexandretran1),
Samantha Nguyen [@clamantha](https://www.github.com/clamantha)

## Data Description 

The Premier League Data Model tracks essential football data over the years, focusing on team performance, wins, losses, and draws. It allows for the analysis of match details like possession, shots on goal, and attendance figures, while also considering factors such as referee assignments and their impact on games. Additionally, the model examines geographical elements, such as stadium locations, and financial aspects, including sponsorship data, to explore how these factors influence the teams success. This model provides valuable information into Premier League football.

## Data Model Description

The Premier League Data Model mostly revolves around the relationships of Teams. Teams has the names of the Football Clubs and year established in the Premier League. The Teams table has an idetifying relationship with Games creating the teamGames entity. The TeamGames entity contains information about which two teams are playing at a given time and includes the statistics belonging to each individual game. TeamGames then has a One to Many relationship with Games which dictates the date of the game and the head referee involved in calling the game. 

Games contains two one-to-one relationships and one one-to-many relationship. The first one-to-one relationship is with referee stating the head referee and first name, last name, and their career start date. The other one-toone relationship is with attendance. This shows how many spectators are expected within one game and the actual amount that was in attendance. A game can have one stadium, but a stadium can have many games creating the Stadium entity. This lists the stadium name its capacity. This also creates a one-to-one relationship with location. This displays the city and state that the stadium is located in. The other branch that stadium has is a one-to-many relationship back to Teams stating that a stadium can have many teams, but a team belongs to only one stadium.

Teams contains three more additional relationships. The first relationship is that a team has many players, but a player only has one team. The second is that a team can have many sponsors, but a sponsor only has one team. The final relationship within teams is that a team has only one manager and a manager has only one team. The entity of players contains basic information about a specific player on a specific team including first and last name, date of birth, and position. The sponsor involved with a team has the company name alongside how much their contract is worth within their association with an organization. The final entity within the data model is the manager entity. This contains information about their first and last name as well as their date of birth.

![new.data.model](https://github.com/user-attachments/assets/82f4356b-e8d1-4b76-a93b-efc141f4934e)

## Data Dictionary

## Queries
Complex Query #1

The first query displays the average expected attendance (in the thousands) compared to the average actual attendance. This can allow the analysis of how much of a difference in expected and actual amount of presence within the game. The ticket office can use this data to track how many people are attending the games, and whether to contact the advertising team to get the word out. If actual attendance is lower than expected, income will be greatly lowered for the team, so it is important to monitor fan attendance.

![query.1](https://github.com/user-attachments/assets/5c3113f6-2f97-42bd-a92d-0ad32105e8e6)

Complex Query #2

The second query shows which team has the highest amount of goals within the season. Goals are key to monitor because it can show how much of an impact a striker is having within a given team. Typically higher scoring teams will end up higher on the table leading to improved statistics. This also shows which teams play more aggressive and play into the box rather than stalling their opponent out.

![query.2](https://github.com/user-attachments/assets/ee9a0d7c-6121-45f5-ba42-bd18adbaa590)

Complex Query #3

The third query informs the user of which stadiums has the highest average attendance. This is key to understanding which teams are performing the best and has the most active fanbase. Lesser performing stadiums  might take a page from the better performing to learn how to better reach their fans and bring them to the stadium. The better performing stadiums gets to monitor their attendance and gauge it against how many people they could increase it by.

![query3.0](https://github.com/user-attachments/assets/280d46c5-0134-4982-8b63-e7f2474926d0)

![query.3.5](https://github.com/user-attachments/assets/9abb425a-74e9-435d-af8c-a9d79fcbc2f1)

Complex Query #4

The fourth query answers the question of how many games had a possession rate over 60% for the winning team. This is important for analysts to recognize because it shows dominance in all areas of play. The winning team showed an impressive win by shutting out the opposition. This win also displays greatly what a team's play style is and how they prioritize keeping the ball in their possession and its efficiency. 

![query.4](https://github.com/user-attachments/assets/27b43bf9-0b11-4a69-9d19-0cfc8334a1c3)

Complex Query #5

The fifth query asks if there is a correlation between average possession time and their total number of wins within the season. This query coincides with the previous one and allows the analysis of whether possession is crucial for a win. Coaches may use this information to their strategic advantage and implementing more possession time into their practice. This can also identify outliers of high possession and low total wins to see if there actually is a correlation between the two. 

![query.5](https://github.com/user-attachments/assets/08e34aea-0382-44cf-8e72-e81b5775f102)

Complex Query #6 

The sixth query asks how many games were overseen by referees with more than 5 years of experience, and what is the average number of goals scored in these games. This query is important to address the integrity of the games played. The referees with more experience are being evaluated for how many goals are allowed during their games. This can be caused through off side calls and different penalty kicks. This can also affect how players play as a referee's tendencies can be learned and used to teams advantages.


![query.6](https://github.com/user-attachments/assets/9bfba032-6629-47a3-a0fd-2efef139719f)

Simply Query #1

The seventh query finds which player has the most goals within the season. This details the performance of that player, but it also provides vital advertising and sales information. The leading scorer is going to gain mass media attention leading to jersey sales and increased sponsorship. A team having the highest scoring player will gain more profits for their club and increase their cap space for signing new players.

![query.7](https://github.com/user-attachments/assets/d008db7b-777b-4a73-a4af-fc70882cd2e1)

Simple Query #2

The eighth query for the Premier League data model finds all team managers and how many team goals they have. This can show how impactful a coach is within their team. How many goals a team has can also indicate the playing style that is tought by the coach. A higher scoring team may have a more aggressive coach towards racking up point totals. The same can be said for lower scoring teams showing either a patient defensive team or a coach that needs to be reevaluated.

![query.8](https://github.com/user-attachments/assets/5bba5cd2-6932-4c38-9ff8-63ef53ade064)

Simple Query #3

The ninth query for the data model is what is the team with the highest contract sponsorship. This displays the team with a high incoming investment into their team. The contract can lead to further investments into their team, back into the stadium, or merchandising to further push their brand. A large discussion of soccer is whether a larger budget for a team increases the likelihood for a championship title, and this query addresses that question.

![query.9](https://github.com/user-attachments/assets/652fcf58-3247-4ab1-a4f0-997941c6f4e5)


Simple Query #4

The tenth and final query of the database is what are the teams with the highest expected attendance. This is key for away teams to understand how loud and populated a stadium is going to be. Crowd noise is always a key factor within sports, as it can interrupt communications between players. This shows where the hardest places to play are and lets away teams prepare for the amount of noise to expect. This also affects the home teams within these stadiums as it sets a standard for practice within the week.

![query.10](https://github.com/user-attachments/assets/d55d3689-e0a5-4799-aedd-87976f5959f2)


## Database Information






