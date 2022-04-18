# Game-Industry-analysis-in-covid-19

This project is a project to visualize and analyze changes in game industry before and after covid19.

Team-project of 'Electronic Manufacturing Data Analysis' lecture in 2021-2

<br> 

I will separate and refactoring code files soon.

<br>

---

## Dataset


| Data                       | Information                                                                           | Analysis                                                        | Source                                                 |
| -------------------------- | ------------------------------------------------------------------------------------- | --------------------------------------------------------------- | ------------------------------------------------------ |
| Vgchart                    | Video Game Sales Through 2020 Data                                                    | regional sales                                                  | kaggle data(https://www.kaggle.com/datasets/baynebrannen/video-game-sales-2020)                                            |
| Player, Twitch viewer data | Steamdb Number of players and number of twitchviewers for games in the top 200 charts |  check the trend of change in player, twitch viewer             | collection with crawling (2018~2020)                   |
| Game data                  | Game Genre and Tag data                                                               | Genre and Tag Changes Before and After Covid-19                 | kaggle data(https://www.kaggle.com/datasets/jesneuman/pc-games)                                            |
| Review count               | Review count of GTA5, Counter Strike: Global Offensive                                | changes in the number of reviews before and after Covid-19      | collection with crawling                               |
| Review data                | Review Data of GTA5                                                                   | keyword and review sentiment analysis before and after covid-19 | before data: steam(Kaggle)https://www.kaggle.com/datasets/luthfim/steam-reviews-dataset   <br> after data: steam(crawling) |


<br>
<br>

---

## Analysis

### 1. Vgchart data

    Sales Pie Chart by Region

    ![00sales](/image/00sales.png)   ![10sales](/image/10sales.png)

    High proportion of sales in English-speaking countries -> Use review data from English-speaking countries for future analysis


### 2. Player, Twitch viewer data

    Trend Analysis of Players and Viewers by Moving Average

    ![moving](/image/viewer_moving.PNG)

    player (blue line) has increased since covid-19(right side of red line), and the switch viewer (orange line) has shown an explosive increase.

### 3. Game data

    Frequency Ranking Bar Chart for Genre and Tags

    Genre
    
    ![before_genre](/image/before_genre.png) ![after_genre](/image/after_genre.png)

    Tag

    ![before_tag](/image/before_tag.png) ![after_tag](/image/after_tag.png)

    Indie games are consistently at the top, and the proportion of action adventures has increased.
    
    Therefore, review analysis uses GTA5, an open world action adventure game.

### 4. Review count

    Review count timeseries graph

    ![gta_review_count](/image/gta_review_count.PNG) ![cs_review_count](/image/cs_review_count.PNG)

    Blue represents positive and orange represents negative reviews. If you look to the right with the color red, you can see that the number of reviews has exploded.

### 5. Review data

    GTA5 review sentimental analysis - using vader

    Positive/Negative Pie Chart

    ![before_sent](/image/before_sent.png) ![after_sent](/image/after_sent.png)

    Positive rate very high after covid-19
     

 
<br>

---

## Keyfile
```Analysis.ipynb``` - It contains all the processes of data loading, preprocessing, and analysis. It will be separated by each data and analysis.

