# Baseball: Homerun Analysis

## Project Goal/Business Understanding
This project aims to analyze the relationship between a player's height and their hitting power.

## Data Understanding  

### Data Preparation
This data comes from the [Lahman Database](http://seanlahman.com/download-baseball-database/) which provides baseball statistics from 1871-2021. Specifically, I used the 'Batting' and 'People' .csv files from the database which include batting statistics (at bats, hits, singles, etc.) and biographical information (date of birth, first name, height, etc.) respectively. 

Within the 'Batting' file, I used the `.groupby()` and `.sum()` functions to aggregate career batting statistics for each player including:
* Career Homeruns (`career_hrs`)
* Career At Bats (`career_AB`)

Within the 'People' file, I used two columns for my analysis, which included variables about:
* player height (`height`)
* player weight (`weight`)

The variables `height` and `weight` show nearly identical correlations to the target of career home runs (`career_hrs`). 

## Exploratory Data Analysis
The analysis including scatterplots and calculation of Pearson's correlation coefficient show that weight and height are nearly identically correlated with career home runs. The correlation coefficient value between height and homeruns (r = 0.527) shows a moderate, positive relationship, and the correlation coefficient value between weight and homeruns (r = 0.530) also shows a moderate, positive relationship. 

## Conclusion
From this analysis, one would expect taller players and heavier players to hit more home runs over their entire career. This makes sense when simply considering Newton's Second Law of Physics (Force = Mass x Acceleration). Heavier players, who are usually taller as well, (height and weight had a correlation coefficient of 0.658) have more mass which allows them to apply more force when they connect with the ball causing the ball to travel farther.

### Limitations
This analysis uses metrics that are readily available for free online, such as height, weight, and number of extra base hits. Nowadays, most Major League Baseball (MLB) organizations have technology that provides advanced metrics (such as bat speed and launch angle) which help measure a player's power potential. This type of data is not as readily available to public users, so while my analysis provides factors that are related to a player's hitting power, MLB organizations may have data that indicates factors that are more strongly correlated with hitting power. In other words, the common readily available data that I used in this analysis may not provide as much insight into which factors are most strongly correlated with a player's hitting power as would data that MLB organizations use.

### Recommendations
The implication for this analysis means that when scouts and coaches are deciding on which players to make up their team, height and weight are criteria that can be used to help evaluate the player’s ability to hit the ball hard and far. Although height and weight are factors when projecting a player’s power potential, there are other factors that should also be considered such as: bat speed, launch angel, overall strength, and how often a player’s swing makes solid contact with the pitch.

### Next Steps
For future iterations of this project, I am interested in performing hypothesis tests to determine if the relationship between a player's height and number of career home runs is statistically significant. Additionally, I plan to explore more up-to-date features that are used to determine a players hitting power potential, such as average exit velocity and barrel percentage.
