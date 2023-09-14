# Project Details

The primary objective of this study was to predict the outcomes of NFL games for the 2021 season, with a particular focus on the spread, total, and overall result of each game. To accomplish this, a comprehensive approach to data sourcing and processing was employed.

The foundation of our data-driven analysis was the play-by-play data sourced from the NFLfastR repository. This data was meticulously aggregated at the game level using the “GAMEID” variable, ensuring each game was represented in a single row. This format was crucial for the subsequent predictive modeling phase. During the transformation process, variables were renamed for clarity and ease of understanding. The resulting dataset, termed “total_games”, spanned games from the onset of the 2010 season to the present, encompassing both regular season and playoff matches.

To enrich the analysis, additional data was incorporated. This included offensive and defensive season stats for teams dating back to the 2003 season, all sourced from Pro Football Reference. Recognizing gaps in this data, advanced statistics like interceptions, sacks, and conversion rates were web scraped and integrated into the dataset. This additional layer of detail proved invaluable for model validation. By juxtaposing the per-game stats of the current season against this rich historical backdrop, we ensured our models were both robust and accurate.

An innovative aspect of our approach was the introduction of a new predictor named “conversion advantage”. This metric calculates the 3rd down conversion advantage or disadvantage that the home team has over the away team. The rationale behind this was the pivotal role 3rd down plays often have in a game, determining whether a drive continues or ends. Ultimately, this predictor captured the essence of these crucial moments, serving as a potent indicator of game outcomes.


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**Special Terms**:

Spread = Home Points − Away Points

Total = Home Points + Away Points

Result = 1 if Home Team Wins
         0 if Home Team Loses

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
