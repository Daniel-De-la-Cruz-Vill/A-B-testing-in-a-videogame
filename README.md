
# **A/B testing in a videogame**

![image](https://github.com/Daniel-De-la-Cruz-Vill/A-B-testing-in-a-videogame/assets/157164355/c877ba19-e63b-4772-8d18-02d6cfbaea58)


This project consists of performing an A/B test for two versions of the videogame Cookie Cats, a cat-themed puzzle game. In this game, players progress through multiple rounds that must be completed until they reach a 'gate' level, originally placed at level 30. In this test, the gate was placed at level 40 for a group of players, instead. The company wants to know whether placing the gate at level 40 had an effect on player retention. This type of study is called an A/B test.

The features of the dataset will be the following:

* **userid**: key value assigned to each individual player.

* **version**: version of the game assigned to the user. gate_30 has the gate at level 30 and gate_40 has the gate at level 40.

* **sum_gamerounds**: total number of rounds played after 14 days.

* **retention_1**: categorical feature that tells us whether the player played after the first day.

* **retention_7**: categorical feature that tells us whether the player played after 7 days.


## **Project Structure**

* **Data Exploration**: In this phase, we explore the dataset and create plots to see important trends in the data. We observe some preliminary results before testing for statistical significance.

* **Data Cleaning**: During the exploration process, an extreme outlier (likely representing an input error) was found. This outlier is treated in this segment to avoid having it derail the results.

* **Hypothesis testing**: Here, we use Levene's test to determine whether the samples have similar variances, Student's two-sample t-test to determine whether the difference between sample means is significant, and Chi-squared test to determine which version provided better player retention.

* **Conclusions**: It was found that the version with the gate at level 30 provided higher player retention. However, the difference is only significant after the first seven days, and the number of rounds played is statistically similar between versions.
