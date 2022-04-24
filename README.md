# Phase 1 Project: Film Strategy for Large Company Entering Movie Market
---
## Overview
The purpose of this project is to study the movie industry and generate advice on how a new entrant to the industry might create and follow a strategy that is aligned with corporate interests and will assure success.
![Movie_Business](https://github.com/NazarMohl/FilmStrategy/tree/main/images/Movie_Business.jpg)
---
## Business understanding 
Microsoft is a large, multinational, technology company with a current focus on Software, PCs, Consumer Electronics, and related services. It is now seeing business potential in the creation of original video content and is exploring the creation of a new movie studio. Lacking experience in the art of creating films, Microsoft has engaged us to explore industry movie trends and identify what type of films are successful at the Box Office and to help them formulate a film strategy that is relevant and optimal for their business concerns.
Specifically, the profitability of a movie was analyzed with respect to:
1)	The director  
2)	Production budget  
3)	Length of a movie  
---
## Data understanding 
Considerable movie data is available ranging from objective, unassailable facts to the subjective and anecdotal reviews from both professional and amateur critics. This project pursues an analysis of objective data that ties film characteristics and attributes to a film’s financial performance. 
Two databases were chosen for analysis:
*[ The Internet Movie Database (IMDb)](https://www.imdb.com/)
Provides information on movie title, year of release, running time (length), director, actors, etc. 
*[The Numbers (TN)](https://www.the-numbers.com/)
Provides information on a movie’s financial performance including release date , production budget and domestic and worldwide gross.
---
## Data assumptions and preparation
Often movies are remade with the same title or a movie title is reused for a later distinctly separate movie. We distinguished movies with the same title by the year in which it was released. The exact duplicate entries were removed. 
In the calculation of the average rating, many movies had only a few or few tens of votes while some had many thousands of votes. We felt that to contribute to our analysis, we needed to exclude movies that did not have many votes. We arbitrarily picked 500 votes as the cut-off and only looked at movies that had more than 500 votes.
The TN database contained financial information and had the movie name in common with the IMDb. It had also a full release date as opposed to only the release year in IMDb. We calculated the release year in the TN database as a separate column and then used the movie name and release year to join these two databases. 
The resultant data set contains information on a little over 2,000 movies which is sufficient to identify trends.
Profit was calculated as:
 Profit = (Domestic_Gross  +  Worldwide_Gross)  –  Production_Budget
Profit Percentage = Profit / Production_Cost * 100. 
This Profit Percentage is a key measure which we use to judge success.
---
## Data Analysis
Descriptive statistics were used in the analysis of this data. The average or mean profit percentage was the specific measurement that was applied across the different cross-sections of data and to look for trends. Specifically, the following questions were chosen for the analysis:
Is there a correlation between directors and profitability?
Is there a correlation between budget and profitability?
Is there a correlation between length of movie and profitability?
---
## Results
---
### Top Directors and Profitability
We sorted our data for directors with the most numbers of movies made and discovered that clearly directors who have a longer track record are likely to be more profitable on average.
![Profitability](https://github.com/NazarMohl/FilmStrategy/tree/main/images/Profit_Percentage_by_Director_for_High_Movie_Count.png)
This chart shows that of the top 20 directors by movie count, all of them were very profitable exceeding 100% and couple in the range of thousands of percent. Clearly, there is a correlation between directors with a track record and their profitability.
For reference we have included the following chart to show the numbers of movies made by these directors.
![MovieCount](https://github.com/NazarMohl/FilmStrategy/tree/main/images/High_Count_of_Movie_Releases_by_Director.png)
---
### Directors and Movie Budgets
The previous charts raised the question as to why some directors can be phenominally profitable and others who are known for making well received movies have not earned as high a profit. This chart along with some general knowledge about the directors provides a clue. David Gordon Green is known for making horror movies. Horror movies do not require a high budget because they do not generally require elaborate special effects and since much happens at night or atleast in the dark, the movie sets do not need to be as detailed or intricate. The likes of Steven Spielberg and Ridley Scott are known for Sci Fi movies which definitely require elaborate special effects and the creation of movie sets reflecting the otherworldly environments that are central to the movies. ALmost by definition a Sci Fi has to require a higher budget.
This project did not focus on genre but this data is implying that profitability by genre should be separately investigated.
![Budgets](https://github.com/NazarMohl/FilmStrategy/tree/main/images/Movie_Budgets_of_Directors_with_High_Count_of_Movie_Releases.png)
---
### All Directors and Profitability
The chart will show most profitable directors regardless of number of movies made.
![AllDirectors](https://github.com/NazarMohl/FilmStrategy/tree/main/images/Most_Profitable_Directors.png)
Just looking at profitability without sorting by movie counts, there are many directors that are showing profitability in the thousands of percent, some well over 10,000 percent. However, the number of movies that they have made is limited. Let's also generate the movie count for these most profitable directors. See the next chart below.
![AllDirectorsMovieCount](https://github.com/NazarMohl/FilmStrategy/tree/main/images/Count_of_Movie_Releases_by_Most_Profitable_Directors.png)
So, many of these highly profitable directors have only made one movie. Perhaps, there was some political, societal or environmental anomaly that brought focus on their single movie and it generated a huge percentage of profitability. A single point of data does not indicate a trend. They may continue to make profitable movies or they may be relegated in history as One-Hit Wonders.
---
### Movie Length vs Profitability
This analysis was initiated with the question as to whether other factors like the length of the movie may correlate with profit or lack thereof. This following sorted data set will be used to look at the effect of movie length on profitability.
![MovieLength](https://github.com/NazarMohl/FilmStrategy/tree/main/images/Movie_Length_Vs_Profitability.png)
The top few high profit movies (outliers) are skewing the results. Let's only look at movies under 2K% profit.
![MovieLength](https://github.com/NazarMohl/FilmStrategy/tree/main/images/Movie_Length_Vs_Profitability_Under_2K.png)
Looking at the vast majority of the movies in our original data set, we do not see a strong correlation. There is some loose indication that most movies are under 2 to 2.5 hours. High profits can be generated in a movie of only 1.5 hours. So if the story does not require a long movie there is no need to stretch the movie into that longer timeframe.
---
## Recommendations
We offer the following 3 recommendations:  
- Work with Directors with track records of consistent profit. 
- Give NEW directors a smaller budget to prove themselves. 
- Need to investigate further the effect of Genre on budgets and therefore profitability.
---
## Other Observations
Microsoft has:
•	Diverse product lines.
•	Sells internationally.
•	Has a large international employee base.
Movie decisions may be driven by:
•	Product placement considerations.
•	Overseas markets.
US Market prefers shorter movies . Need to study other markets.
---
## Next Steps
Investigate non-US markets
Identify opportunities for product placement
Formulate marketing strategies to drive product placement
Engage movie industry drivers to consider how to move Microsoft interests further.