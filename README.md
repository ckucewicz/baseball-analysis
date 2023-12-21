# Baseball: Homerun Analysis

## Project Goal
This project aims to analyze the relationship between a player's height and their hitting power.

## Business Understanding

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

## Conclusion

### Limitations

### Recommendations

### Next Steps

