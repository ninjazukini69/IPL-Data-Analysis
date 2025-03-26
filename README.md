# IPL-Data-Analysis
Indian Premier League (IPL) Data Analysis Report: 2008-2018 

1. Introduction 

The Indian Premier League (IPL) is a professional Twenty20 cricket league in India, contested annually in April and May. This report presents an exploratory data analysis of IPL match and delivery data from 2008 to 2018, aiming to identify key trends and patterns in team and player performance, match outcomes, and other relevant factors. 

2. Data Description 

The dataset comprises two primary CSV files: 

matches.csv: Contains match-level information, including: 

id: Unique identifier for each match. 

season: The year the match was played. 

city: The city where the match was held. 

date: The date of the match. 

team1, team2: The two teams competing in the match. 

toss_winner: The team that won the toss. 

toss_decision: The decision made by the toss-winning team (bat or field). 

result: The result of the match (e.g., normal, no result). 

dl_applied: Whether the Duckworth-Lewis rule was applied. 

winner: The team that won the match. 

win_by_runs: The runs by which the winning team won. 

win_by_wickets: The wickets by which the winning team won. 

player_of_match: The player awarded the "Player of the Match." 

venue: The stadium where the match was held. 

umpire1, umpire2, umpire3: The umpires officiating the match. 

deliveries.csv: Contains ball-by-ball information for each delivery within a match, including: 

match_id: The ID of the match. 

inning: The inning number. 

batting_team: The team batting. 

bowling_team: The team bowling. 

over, ball: The over and ball number. 

batsman, non_striker: The batsman and non-striker on strike. 

bowler: The bowler. 

is_super_over: Whether the delivery was bowled in a super over. 

bye_runs, legbye_runs, noball_runs, penalty_runs, batsman_runs, extra_runs, total_runs: Runs scored. 

player_dismissed: The player who was dismissed. 

dismissal_kind: The type of dismissal. 

fielder: The fielder involved in the dismissal. 

3. Methodology 

The analysis was conducted using Python 3.x, with the following key libraries: 

Pandas: For data manipulation, cleaning, and aggregation. 

Matplotlib and Seaborn: For creating visualizations. 

The analysis involved: 

Loading the datasets using pd.read_csv(). 

Exploring the data structure and basic statistics using methods like .head(), .shape, and .describe(). 

Aggregating data to calculate team-wise and player-wise statistics. 

Visualizing trends and relationships using count plots, bar charts, and pie charts. 

4. Results and Analysis 

4.1 Match Overview 

Total Matches and Seasons: The dataset comprises 696 matches played across 11 seasons (2008-2018). 

Matches per Season: The number of matches played per season shows some variation. 

Matches per Venue: The M. Chinnaswamy Stadium, Bangalore, hosted the highest number of matches, followed by Eden Gardens, Kolkata. 

Matches Played by Each Team: Mumbai Indians participated in the most matches, followed by Royal Challengers Bangalore. 

Wins per Team: Mumbai Indians secured the most wins, followed by Chennai Super Kings. 

Champions: The champions for each season from 2008 to 2018 were: Rajasthan Royals, Deccan Chargers, Chennai Super Kings (twice), Kolkata Knight Riders (twice), Mumbai Indians (thrice), and Sunrisers Hyderabad, Chennai Super Kings. 

4.2 Toss Decisions and Match Outcomes 

Toss Decision Preference: Approximately 55% of the teams opted to field first after winning the toss, indicating a preference for chasing. 

Win Percentage Batting Second: Teams batting second won 53.2% of the matches, suggesting a slight advantage. 

Toss Win vs. Match Win: Winning the toss does not guarantee a win. 

Team-wise Toss Impact: Chennai Super Kings demonstrated a higher correlation between winning the toss and winning the match, while Pune Warriors had a negative correlation. 

4.3 Player Analysis 

Top Run Scorers: Virat Kohli is the leading run-scorer, followed by Suresh Raina. 

Most Boundaries (4s): Gautam Gambhir hit the most fours. 

Most Sixes (6s): Chris Gayle hit the most sixes. 

Most Dot Balls Faced: Gautam Gambhir faced the most dot balls. 

Highest Percentage of Dot Balls: Sourav Ganguly had the highest percentage of dot balls (among batsmen who faced more than 200 balls), followed by other players. 

4.4 Bowler Analysis 

Most Balls Bowled: Harbhajan Singh bowled the highest number of balls. 

Most Dot Balls Bowled: Harbhajan Singh also bowled the most dot balls. 

Most Extra Runs Bowled: Lasith Malinga conceded the most extra runs. 

4.5 Dismissal Analysis 

Common Dismissal Types: "Caught" is the most frequent mode of dismissal, followed by "Bowled." 

4.6 Umpire Analysis 

Most Frequent Umpires: Dharmasena officiated in the most matches, followed by S. Ravi. 

5. Discussion 

The analysis of IPL data from 2008 to 2018 reveals several notable trends. Mumbai Indians and Chennai Super Kings have been the most successful teams, demonstrating consistent performance over the years. The preference for fielding first after winning the toss suggests a strategic advantage in chasing targets. Key players like Virat Kohli, Chris Gayle, and Lasith Malinga have significantly impacted the league with their exceptional batting and bowling skills. 

6. Conclusion 

This report provides a comprehensive exploratory data analysis of IPL match and delivery data. The findings offer valuable insights into team and player performance, match dynamics, and other key aspects of the league. These insights can be of interest to cricket analysts, team management, and fans alike. 
