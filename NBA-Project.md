<img src="/images/nba-project-header.png?raw=true" alt="Beyond the Scoreboard: NBA Player and Team Performance in Tableau" width="100%"/>
# Beyond the Scoreboard: Exploring NBA Player and Team Performance in Tableau

[**Explore the interactive Tableau story.**](https://public.tableau.com/app/profile/kevin.felix/viz/NBAStatsTableauProject/AnalysisStory)

## Intro

Basketball statistics can tell us much more than the final score. Looking at how players score, create opportunities for teammates, and contribute at different ages can help us better understand the differences between teams and individual playing styles.

In this project, I used Tableau to explore the 2022 NBA player data shown in my Tableau story. Through a scatterplot, stacked bar charts, and a heatmap, I examined several questions:

- How do scoring and assists differ across player positions?
- Which age groups contribute the most points to each team?
- How is team scoring distributed among individual players?
- How does average three-point shooting percentage vary by team and position?

## Data Analysis

### Comparing Scoring and Playmaking

To begin my exploration, I compared total points and assists in a scatterplot. Each mark represents a player, with points on the horizontal axis, assists on the vertical axis, and color identifying the player's position.

<img src="/images/nba-points-assists.png?raw=true" alt="Scatterplot of NBA player total points and assists, colored by position" width="100%"/>

One of the clearest patterns is the concentration of point guards near the top of the chart. Players such as Trae Young, Chris Paul, and Dejounte Murray stand out for their assist totals. Trae Young also appears at the far right, combining a high scoring total with the highest assist total shown.

An interesting exception is Nikola JokiÄ‡. Although he plays center, his position on the chart places him among players with both high scoring and high assist totals, in an area largely occupied by point guards. This highlights how a player's statistical contributions can extend beyond the expectations associated with their position.

At the same time, these are total statistics. Games played and minutes on the court can affect where a player appears, so the chart describes overall production rather than performance per minute or per game.

### Understanding Each Team's Scoring by Age

After looking at individual production, I explored how different age groups contribute to team scoring. This stacked bar chart separates total points into three groups: under 25, ages 25â€“29, and ages 30 and older.

<img src="/images/nba-team-points-age.png?raw=true" alt="Stacked bar chart of NBA team points split into under-25, 25â€“29, and 30-plus age groups" width="100%"/>

Minnesota has the highest total points in the displayed data, with players ages 25â€“29 contributing the largest portion. Oklahoma City sits at the opposite end of the chart, with most of its scoring coming from players under 25.

Other teams show different patterns. Memphis also receives a large share of its scoring from the under-25 group, while the Lakers receive the largest portion of theirs from players ages 30 and older. Teams with similar scoring totals can therefore have very different age profiles behind those totals.

This comparison provides a useful way to describe a roster's scoring contributions. However, a larger contribution from one age group does not establish that those players are more efficient or that a particular age profile leads to more wins. Roster composition and playing time also influence these results.

### Breaking Team Scoring Down by Player

Age groups provide a broad view, but I also wanted to see the individual players behind each team's total. The next stacked bar chart breaks team scoring into player contributions.

<img src="/images/nba-team-points-player.png?raw=true" alt="Stacked bar chart showing individual player contributions to NBA team scoring totals" width="100%"/>

Minnesota's bar includes substantial contributions from Karl-Anthony Towns and Anthony Edwards. Other examples include Jayson Tatum and Jaylen Brown in Boston, and DeMar DeRozan and Zach LaVine in Chicago.

Viewing the data this way adds context to the previous chart. A team total summarizes production, while the individual segments show how that production is distributed across the roster. It becomes easier to identify prominent scoring contributors and explore how much of a team's total comes from them.

Because each bar contains many players, the interactive Tableau view is especially useful for inspecting individual segments. A separate sorted player chart would be a clearer way to compare scoring leaders directly across the league.

### Exploring Three-Point Shooting by Team and Position

For the final part of my analysis, I created a heatmap comparing average player three-point shooting percentage across teams and positions. The rows represent teams, the columns represent positions, and darker shades indicate higher averages.

<img src="/images/nba-three-point-heatmap.png?raw=true" alt="Heatmap of average player three-point percentage by NBA team and position" width="100%"/>

Several frontcourt groups stand out. San Antonio's centers and Sacramento's power forwards each show an average of approximately 45%. The Clippers also have high averages among centers and small forwards, at approximately 43% and 47%, respectively.

These examples show that high three-point percentage averages in this dataset are not limited to guards. The heatmap makes it easy to identify team-position combinations worth exploring further.

There is an important distinction in how this chart should be interpreted: it uses **AVG(3P%)**, the average of player shooting percentages. That differs from a combined percentage calculated by dividing total three-pointers made by total attempts. A player with very few attempts can influence the average, so these results should be considered alongside shooting volume before drawing conclusions about a group's shooting strength. The `TOT` row is also a separate source-data category and should not be interpreted as an NBA team.

### Final Insights

- Point guards feature prominently among players with high assist totals, while Nikola JokiÄ‡ stands out as a center with strong scoring and playmaking production.
- Teams differ considerably in which age groups contribute their points. Minnesota's largest contribution comes from ages 25â€“29, while Oklahoma City's comes from players under 25.
- Breaking team totals down by player reveals the individual contributors behind each team's scoring output.
- High average three-point percentages appear across several positions, including centers and power forwards.
- Totals and averages answer different questions. Playing time and shooting attempts provide important context for interpreting the patterns shown.

This project helped me use Tableau to move between individual performance and broader team patterns. By combining multiple chart types in one story.

Thank you for taking the time to check out my project! You can [explore the interactive Tableau story here](https://public.tableau.com/app/profile/kevin.felix/viz/NBAStatsTableauProject/AnalysisStory). If you'd like to chat or have any questions, feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/kevinfelixleyva/)!
