# Project_1

This is an analysis of top Spotify tracks in 2023.
We set out to analyze what users are listening to and discover trends and implications so streaming platforms (Spotify, Apple & Deezer) can increase potential revenue.
We used python, matplotlib, pandas, and stats.

# Our Findings:
## Question 1:
In question 1, we were examining the similarities among the number one songs on each platform (Spotify, Apple, and Deezer). Pop music was the most popular genre on all three platforms, and with Rap/Hip Hop closely following. When considering the key of the songs, we found that all keys was evenly distributed. However, when looking at whether the music was in a minor or major key, we’ve noticed that major key was the most popular in Spotify, whereas on Apple and Deezer, minor were more popular. Finally, when it came to BPM, we grouped  the BPMs to have a better idea. The most common BPM range on Spotify was 80-99, which is considered slow in a major key. For Apple, the most common range was 100-110 which is more of a medium-fast tempo. Deezer, on the other hand, had the fastest tempo, with the most common BPM range being 120-130.


## Question 2:
In question 2, we were interested in looking into the top 3 songs in each platform based on how many playlists a song was saved in.

<img width="950" alt="Screenshot 2023-10-11 212753" src="https://github.com/RobinLWilson/Project_1/assets/141863731/693b985b-d05a-4ebd-8c7f-156dbbb43062">

Then we looked into the 3 top songs based on Spotify Streams. Also, we created a bar chart to see which artist has the most saved songs.

<img width="475" alt="image" src="https://github.com/RobinLWilson/Project_1/assets/141863731/0f664098-84d4-4f53-834b-a97dba882b50">
<img width="521" alt="Screenshot 2023-10-11 213832" src="https://github.com/RobinLWilson/Project_1/assets/141863731/0636b672-6a27-491c-809a-bac35dd5663f">

Finally, for part 2, we created another bar chart to see which months top songs were released in.
<img width="409" alt="image" src="https://github.com/RobinLWilson/Project_1/assets/141863731/f3ff3717-69f8-4afb-9e98-0e03eb96e649">

## Question 3:
In Question 3 we looked at what songs charted on all three platforms and analyzed them by genre, bpm, and key(major v. minor). This was done by reducing the dataset and removing any song that did not chart on all three platforms, deezer, apple music and Spotify. Begining with key, we first looked at how many songs charted for each key, and found these results.  <img width="616" alt="image" src="https://github.com/RobinLWilson/Project_1/assets/142050568/5e33ebca-8aaa-4cbf-9724-3b6c63d29920"> While that did not tell us much about the songs, we grouped them by major v minor songs, where major songs are more cheerful songs and minor songs are typically sadder and calmer. <img width="417" alt="image" src="https://github.com/RobinLWilson/Project_1/assets/142050568/23d23f27-476b-4db7-87e6-b398fe7b6a2b"> This chart shows that songs in a major key charted on all three platforms more often than songs in a minor key. Next, we analyzed bpm. According to the following chart we found that charted songs have a variety of bpms, but bpms that had 5 or more songs chart are typically within 100-180 bpm. <img width="606" alt="image" src="https://github.com/RobinLWilson/Project_1/assets/142050568/b934ae0c-8a04-488d-b83c-f3a8ac20c65d"> 
Lastly, we looked at genre. The genre with the most songs that charted on all three platforms was pop followed by rap/hip hop. <img width="576" alt="image" src="https://github.com/RobinLWilson/Project_1/assets/142050568/d08beb5e-8872-42d7-815e-3496d95fcc07"> 

Based on these findings, in general, songs that are in a major key, between 100-180 bpm and pop songs chart the most.

## Question 4:
Question 4 looks at songs streamed in 2023 by their release year. 

We see that songs released in 2023 represent only 6% of streaming, songs released in 2022 represent 26% of streaming and songs released before 2022 represent 68% of streaming.  An Anova test and p-value told us there is a statistically significant difference between year groups.
![Streams by Release Year](https://github.com/RobinLWilson/Project_1/assets/139357402/dc4d9dd1-159a-4f7a-a7ee-2e246db7e862)

When looking at the genre by release year groups we see that users are listening to mostly rap & hip/hop in 2023 releases, and pop in 2022 and before 2022 releases.  While this may be important in building the user profile, an Anova test & p-value show us this is not statistically significant.
![Popularity of Songs Released in 2023 by Genre](https://github.com/RobinLWilson/Project_1/assets/139357402/639d55a6-a54b-4862-a4c3-6cf50749f231)
![Popularity of Songs Released in 2022 by Genre](https://github.com/RobinLWilson/Project_1/assets/139357402/817de64e-9bf5-47f7-ae05-6ffd2f5b7c45)
![Popularity of Songs Released Before 2022 by Genre](https://github.com/RobinLWilson/Project_1/assets/139357402/94cd6e9e-fb37-4a52-a132-3338d4a9a805)

When looking at Major versus Minor in year groups we see that 2023 releases are mostly in the minor key while songs released in 2022 and before 2022 are mostly in the major key.  A Chi2 and Contingency test of key between year groups shows a p-value of 2.49%- therefore there is a statistically significant association between key and year.
![Songs from 2023 by Mode](https://github.com/RobinLWilson/Project_1/assets/139357402/f68d67a3-83ca-4849-9913-75c073d732b9)
![Songs from 2022 by Mode](https://github.com/RobinLWilson/Project_1/assets/139357402/d8f64df6-eb4f-4708-840a-2f380d507b0a)
![Songs from Before 2022 by Mode](https://github.com/RobinLWilson/Project_1/assets/139357402/b9b93396-b4cb-4cb5-8850-32d6128e3aaf)

When looking at BPM between year groups, we see the average is 120.  I conducted a t-test and the resulting p-value said there was not a significant association.
![Songs from 2023 by BPM](https://github.com/RobinLWilson/Project_1/assets/139357402/6f8c14b9-8c93-4468-88fc-349ae5e7eeb3)
![Songs from 2022 by BPM](https://github.com/RobinLWilson/Project_1/assets/139357402/0082e1e1-bd80-44ed-a9fb-6027943d1854)
![Songs from Before 2022 by BPM](https://github.com/RobinLWilson/Project_1/assets/139357402/3addbae5-7bf6-4269-8eab-a1695eeedd47)
![Songs by BPM by Years](https://github.com/RobinLWilson/Project_1/assets/139357402/6099d491-755b-4d73-8ecc-e35a4f8899ad)

### NOTE:
This was a collaborative project between 4 data science students:
Alaa A: alaaaleryani31@gmail.com
Amanda K: krestamanda@gmail.com
Tiffany Y: hsyuk0618@gmail.com
Robin W: wilson.robin.leigh@gmail.com

Acknowledgements:
Nidula Elgiriyewithana: Top Spotify Songs data set: https://www.kaggle.com/datasets/nelgiriyewithana/top-spotify-songs-2023/

RapidAPI and Deezer: API call to find the genres: https://rapidapi.com/deezerdevs/api/deezer-1

SlidesGo: presentation template: https://slidesgo.com/theme/lofi-music-album-pitch-deck 
