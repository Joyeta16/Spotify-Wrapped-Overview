# Music by the Numbers: Spotify Wrapped Analysis  


## Project Objective:

To create a personalized Spotify Wrapped dashboard that provides a comprehensive view of the user's listening habits over the years. The dashboard will showcase trends in listening behavior by year, month, weekday, and time of day, while also highlighting personal music preferences, such as favorite artists, tracks, and albums. The goal is to deliver an engaging, data-driven summary of the user's unique music journey.

## Dataset

The data for this project is sourced from the Maven Analytics website and can be accessed via the following link:
[Maven Music Challenge](https://mavenanalytics.io/challenges/maven-music-challenge/e161353d-9967-4297-869c-505de168e610)

It contains two CSV files:

1. spotify_data_dictionary: A reference file describing the dataset's columns.
2. spotify_history: The primary dataset used in this project.

The spotify_history file includes detailed information such as:

- spotify_track_uri: Unique identifier for each track.
- ts: Timestamp (in UTC).
- platform: Platform used for streaming the track.
- ms_played: Playback duration in milliseconds.
- track_name: Name of the track.
- artist_name: Artist of the track.
- album_name: Album of the track.
- reason_start: Reason the track started playing.
- reason_end: Reason the track stopped playing.
- shuffle: Shuffle status (True/False).
- skipped: Skipped status (True/False).

This dataset forms the foundation for analyzing listening habits and uncovering music preferences.

Data Cleaning Process

Summarize the steps taken to clean and prepare the data:
Removed duplicates or irrelevant records.
Transformed timestamps into meaningful time formats (e.g., months, weekdays, hours).
Created calculated metrics (e.g., play duration, skipped tracks).
Addressed missing values or inconsistencies.

