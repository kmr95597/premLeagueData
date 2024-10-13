# premLeagueData

## Group Name:
29704 Group 9

## Team Members:
Kevin Reilly,
Alex Tran,
Samantha Nguyen

## Data Description 
The Premier League Data Model tracks essential football data over the years, focusing on team performance, wins, losses, and draws. It allows for the analysis of match details like possession, shots on goal, and attendance figures, while also considering factors such as referee assignments and their impact on games. Additionally, the model examines geographical elements, such as stadium locations, and financial aspects, including sponsorship data, to explore how these factors influence the teams success. This model provides valuable information into Premier League football.

## Data Model Description
The Premier League Data Model mostly revolves around the relationships of Teams. Teams has the names of the Football Clubs and year established in the Premier League. The Teams table has an idetifying relationship with Games creating the teamGames entity. The TeamGames entity contains information about which two teams are playing at a given time and includes the statistics belonging to each individual game. TeamGames then has a One to Many relationship with Games which dictates the date of the game and the head referee involved in calling the game. 

Games contains two one-to-one relationships and one one-to-many relationship. The first one-to-one relationship is with referee stating the head referee and first name, last name, and their career start date. The other one-toone relationship is with attendance. This shows how many spectators are expected within one game and the actual amount that was in attendance. A game can have one stadium, but a stadium can have many games creating the Stadium entity. This lists the stadium name its capacity. This also creates a one-to-one relationship with location. This displays the city and state that the stadium is located in. The other branch that stadium has is a one-to-many relationship back to Teams stating that a stadium can have many teams, but a team belongs to only one stadium.

Teams contains three more additional relationships. The first relationship is that a team has many players, but a player only has one team. The second is that a team can have many sponsors, but a sponsor only has one team. The final relationship within teams is that a team has only one manager and a manager has only one team. The entity of players contains basic information about a specific player on a specific team including first and last name, date of birth, and position. The sponsor involved with a team has the company name alongside how much their contract is worth within their association with an organization. The final entity within the data model is the manager entity. This contains information about their first and last name as well as their date of birth.





