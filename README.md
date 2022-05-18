# DS3000Project_Group30

Vivek Divakarla, Daniel O'Connor, Abyan Nawaz

Research on Spreads and Moneylines for the 2020-2021 NBA Season. 

Project for DS3000 - Foundations of Data Science

The goal of our project is to predict if the home team covers the spread in a certain basketball game to help sports bettors. We
would also like to learn more about Vegas odds and how they skew odds in their favor. Using our predictions
and our gained insight on Vegas odds, we can better identify which betting lines are poorly constructed and
could be exploited. In essence, this would create a “money machine” that could repeatedly predict strong bets
for bettors to take advantage of.

Our dataset represents all NBA games from the 2020-2021 season. We have a few target variables, since
there are multiple items to bet on. These targets include money line data, spread, turnover percentage, effective field goal percentage per team and many more.  With these multiple features, we can analyze which teams are most likely to “cover the spread”which teams are likely to contribute to a higher total score, which teams are most consistent to win as the favorite, etc. Using machine learning algorithms, we will be able to create a model that predicts whether a team covers the spread or not, as described above, and exploit certain aspects of it to hopefully, obtain a positive cash flow.

<img width="423" alt="Screen Shot 2022-05-18 at 4 37 31 PM" src="https://user-images.githubusercontent.com/11672096/169151441-2050bab9-6bfc-4af4-ba80-3f9e4b617caa.png">

This graph is showing a distribution of the Odds for each game of the 2020-2021 NBA season

<img width="607" alt="Screen Shot 2022-05-18 at 4 37 54 PM" src="https://user-images.githubusercontent.com/11672096/169151494-04caac75-2650-4e75-bf72-b8b04476cae7.png">

In this graph here, “Home Team Versus Away Team Score in Relation to Covering the Spread,” there is an interesting point to be made about the distribution of points. Each point on the graph represents an NBA game played in the 2020-2021 season. The y-axis in this graph is the home team’s final score, and the x-axis represents the away team’s final score. This can be interpreted as if a point seems higher on the graph than it is to the right, the home team wins. The color of each dot is important to note as well, the blue color represents when the home team does not cover the spread. The orange dot represents when the home team does cover the spread.

<img width="398" alt="Screen Shot 2022-05-18 at 4 38 24 PM" src="https://user-images.githubusercontent.com/11672096/169151577-2a3b62eb-c500-42ab-954b-bd9da6eaa887.png">

In this graph we are comparing a teams effective field goal percentage with the number of wins they had in the regular season. On the y-axis we have the EFG% and the x-axis we have the total wins per team. Each dot on the graph represents a team. We see a pretty strong positive correlation between these two variables. The higher the teams EFG% is the more wins they will have. This is super important for our model as we are essentially trying to figure out which team is going to win. This EFG% stat is basically the % of shots that a team takes that goes in, so with that being said, if you make more than 56% of your shots, you are most likely going to win a lot, and we see this reflected on the graph.

# Results
<img width="502" alt="Screen Shot 2022-05-18 at 4 43 32 PM" src="https://user-images.githubusercontent.com/11672096/169152407-366915d6-d173-4f33-b44a-6f9d7342b203.png">

The algorithms we should use for this problem would be Gaussian Naive Bayes. This model can be used to predict if the home team covers the spread, but it should not be the only factor if you were to make a smart decision. The model predicts with ~60% accuracy which is better than a coin flip, so statistically speaking, you would net profit if the model was true to this nu![Uploading Screen Shot 2022-05-18 at 4.43.18 PM.png…]()
mber, but as we know in statistics, this is not always the case. All in all, you should use this model as another factor in your decision, one that has a good amount of weight but, not your only telltale sign.
