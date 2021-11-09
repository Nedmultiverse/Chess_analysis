# Chess_analysis
Project used to practise python and data analysis. 

The project starts by using the chessdotcom package to pull the relevant data. This is stored as a .txt JSON format file - it's a mess and useless without processing. Processing included reformatting the data, then coding to extract the data from the .txt and store as a dictionary. This dictionary was then converted into a DataFrame (using Pandas). The analysis is ongoing - as well as a tiny bit of modelling at the end :) This has been my method of becoming more familiar with python - some of the code may well be quite inefficient - very open for suggestions to improve and any insights you think could be interesting to find!




Insights gleamed so far..
- I suck at e4 openings compared to d4 (avg result of 0.05 vs 0.16, where 1=win, draw = 0, loss = -1, we'd expect average to around 0)
- I am really bad at the Caro-Kahn (I knew this already.. the advanced variation kills me)
- My best opening (specific line) is the Queens-Gambit-Accepted-Central-Variation with an average result of 0.41 - I put down the opponent within just 9.6 mins avg.
- 1% of all my games have been the Ruy Lopez opening with an avg result of 0.5
- If I win my previous game, I hankering to play again - it takes me 70% of the time before my next game compared to if I lose the last game.
- Unsurprisingly, my most efficient opening (judged by ELO gained per minute playing) is the the Queen's-Gambit-Accepted: with a whopping 0.03 ELO points per minute.
- If I am running low on time but I want to fit a game in, I should open with e4 (avg length of 10.3 mins). If I open with d4 the game takes on average 40 seconds longer.
- If I win or lose a game, it doesn't have much impact on my likelihood to win/lose the next game, however if I draw a game, I am more likely to lose the next game.
- Saturday is my best day to play (win rate of 0.52) vs Tuesday which is my worst day to play (win rate of 0.46)
- I spent a lot of time trapped around 1000 elo, then when I finally came through I progressed to 1400 quickly, where I again remain trapped.
- On average, if I drew a game my ELO is was 3 more than my opponent, 28 more for a win, and 22 less for a loss.
- I've spent an average of 42 minutes playing 10 minute games per day since my first game! (About 4 games).
- Average game length is 10.3 minutes.
- I average 5.5 games on Saturday (max) and only a pitiful 3.8 games on a Tuesday.
- 

Chess.com scraping -> wrangling -> analysis
