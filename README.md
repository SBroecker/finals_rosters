# NBA Finals Rosters

A repo containing code to check how many years a player from each team played in the NBA finals. Inspired by the stat from reddit that all 75 years of the NBA have featured a finals with at least one player who is a current, past, or future Knick.

The final output of this code is `teams_per_year.csv`, which contains a row for every year of the NBA finals and a column for each NBA team. The column for a team is 1 if a player who ever played on that team was in the finals that year and 0 otherwise.

## `scraping.ipynb`

All the code is in here. The general flow of the code is:

1. Get the two teams in every NBA finals matchup from Basketball Reference.
2. For every team in every finals, get all of the players from those teams.
3. For every player for every team in every finals, get all of the teams they every played for.
4. Aggregate all of the teams represented in every year of the finals.