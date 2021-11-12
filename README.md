# Project Details
This is a predictive modeling project related to the world of sports betting in the NFL. The primary goal of this project is to design models for prediction of three variables – Spread, Total, and Result – often used in sports gambling. Our group made predictions of the three variables for all NFL games between November 8 and November 29, inclusively.

Spread = Home Points − Away Points

Total = Home Points + Away Points

Result = 1 if Home Team Wins
         0 if Home Team Loses

To build adequate predictive models, we need to use historical data for training and testing. The dataset "game_results.csv" contains important information about every game in the NFL since 1966. The dataset "nfl_stadiums.csv" contains information on all NFL stadiums. The dataset "nfl_teams.csv" contains important information necessary for linking datasets according to team name and abbreviations. 

Since the data we are given is elementary and basic, we also engineered a new variable and used outside data (more details can be found in the report pdf file), which helped us gain a competitive edge in the sports betting market.

Glossary
Rk -- Rank This is a count of the rows from top to bottom. It is recalculated following the sorting of a column.
G -- Games played

Points
PF -- Points Scored by team (on defensive datasets this represents points allowed)

Tot Yds & TO
Ply -- Offensive Plays: Pass Attempts + Rush Attempts + Times Sacked
Y/P -- Yards per Offensive Play
(Rush + Pass Yards)/( Pass Attempts + Rush Attempts + Times Sacked)
TO -- Takeaways
FL -- Fumbles Lost by Team
1stD -- First Downs

Passing
Cmp -- Passes completed
Att -- Passes attempted
Yds -- Yards Gained by Passing
For teams, sack yardage is deducted from this total
TD -- Passing Touchdowns
Int -- Interceptions thrown
NY/A -- Net Yards gained per pass attempt (Passing Yards - Sack Yards) / (Passes Attempted + Times Sacked) Minimum 14 attempts per schedule game to qualify as leader. Minimum 1500 pass attempts to qualify as career leader.
1stD -- First Downs by Passing

Rushing
Att -- Rushing Attempts (sacks not included in NFL)
Yds -- Rushing Yards Gained (sack yardage is not included by NFL)
TD -- Rushing Touchdowns
Y/A -- Rushing Yards per Attempt Minimum 6.25 rushes per game scheduled to qualify as leader. Minimum 750 rushes to qualify as career leader.
1stD -- First Downs by Rushing

Penalties
Pen -- Penalties committed by team and accepted
Yds -- Penalties in yards committed by team
1stPy -- First Downs by Penalty

Percentages
Sc% -- Percentage of drives ending in an offensive score
TO% -- Percentage of drives ending in an offensive turnover

Expected Points
EXP -- Expected points
