### README

This is an additional folder to provide extra information related to our website https://fpl-wizard.web.app/

#### About the website

The website is designed to always predict the best combination of 11 players (typically called dream team) for the next gameweek in the game Fantasy Premier League.

Thus, the website can be used as a decision support system to help out with decisions like:
- Which players should one prioritize to swap into your team before next gameweek?
- Which player should you make your captain the next gameweek? (Captains earns double points, so you would want your highest scoring player to be captain)
- And lots of other stuff we are sure.

#### Predicting the next dream team

The machine learning models built in this project predicts the points next gameweek for every player. 
A dream team would be the highest scoring team.
However, in addition to maximize the predicted points of the players there also applies some constraints (by the rules of the game):
- A maximum amount of money spend (every player cost a given amount of money).
- A proper formation (for example you can only have one goalkeeper).
- A maximum of three players from each of the real world teams.

This constrained optimization problem is solved by the Simplex algorithm.
The details of the Simplex algorithm is beyond the scope of this README, but in short it is a linear programming optimzation technique for solving problems like the one outined above. Also, we should mention that we use the pulp library for the Simplex optimization.


###### To summarize the pipline:
Each week do:
1. Fetch and preprocess data
2. Build and train models
3. Collect data for the upcoming gameweek
4. Predict points for all players
5. Formulate consatraind optimization problem and solve by the Simplex method to construct the predicted dream team


The code for step 1 - 4 is provided in the file SimplexFPL_preprocessing.
The code for step 5 is provided in the file SimplexFPL.


