# SQL Solution


```select 
user_id,
sum(listen_duration/60) as total_listen_duration,
count(distinct(song_id)) as unique_song_count
from listening_habits
group by 1
