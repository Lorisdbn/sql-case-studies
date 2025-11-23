
# 🎮 Analyzing the Golden age of video games

![video_game](video_game.jpg)

Video games are big business: according to **Mordor Intelligence**, the global gaming market is projected to exceed **$300 billion by 2027**. With so much money at stake, major publishers are highly motivated to create the next big hit.

But are games actually getting better, or has the golden age of video games already passed?

In this project, I will analyze **critic and user scores**, along with **sales data**, for the **top 400 video games** released since 1977. Goals:

- Identify the **best-rated release years** (the “golden age”).
- Explore the **business side** of gaming through sales figures.

> 💡 Note: Each table has been limited to 400 rows for this project. 

## 📊 Tables Overview

### Table: `game_sales`

| Column      | Definition                                 | Data Type |
|-------------|---------------------------------------------|-----------|
| name        | Name of the video game                      | varchar   |
| platform    | Gaming platform                             | varchar   |
| publisher   | Game publisher                              | varchar   |
| developer   | Game developer                              | varchar   |
| games_sold  | Number of copies sold (in millions)         | float     |
| year        | Release year                                | int       |

---

### Table: `reviews`

| Column       | Definition                                 | Data Type |
|--------------|---------------------------------------------|-----------|
| name         | Name of the video game                      | varchar   |
| critic_score | Critic score (from Metacritic)              | float     |
| user_score   | User score (from Metacritic)                | float     |

---

### Table: `users_avg_year_rating`

| Column         | Definition                                          | Data Type |
|----------------|-----------------------------------------------------|-----------|
| year           | Release year of reviewed games                      | int       |
| num_games      | Number of games released that year                  | int       |
| avg_user_score | Average user score for that year’s games            | float     |

---

### Table: `critics_avg_year_rating`

| Column           | Definition                                         | Data Type |
|------------------|----------------------------------------------------|-----------|
| year             | Release year of reviewed games                     | int       |
| num_games        | Number of games released that year                 | int       |
| avg_critic_score | Average critic score for that year’s games         | float     |
