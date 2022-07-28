# Data-Modeling-for-a-music-streaming-App
## Create a Postgres database with tables designed to optimize queries on song play analysis
> A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The analytics team is particularly interested in understanding what songs users are listening to. Currently, they don't have an easy way to query their data, which resides in a directory of JSON logs on user activity on the app, as well as a directory with JSON metadata on the songs in their app

### using the song and log datasets, I've created a star schema optimized for queries on song play analysis. This includes the following tables.
### Fact Table

    songplays - records in log data associated with song plays i.e. records with page NextSong

    songplay_id, start_time, user_id, level, song_id, artist_id, session_id, location, user_agent

### Dimension Tables

    users - users in the app

    user_id, first_name, last_name, gender, level

    songs - songs in the music database

    song_id, title, artist_id, year, duration

    artists - artists in the music database

    rtist_id, name, location, latitude, longitude

    time - timestamps of records in songplays broken down into the specific unit

    start_time, hour, day, week, month, year, weekday
