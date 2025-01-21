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

The analysis covers data from 2013 to 2024, offering valuable insights into listening habits and personal music preferences.

## Data Cleaning Steps

### Used Power Query to Clean the Data:  

- Cleaned and transformed the dataset using Power Query to prepare it for analysis.

### Created Columns for Duration:

- Extracted seconds and minutes from the ms_played column to better understand playback duration.

### Extracted Date Information:

- Extracted the date from the ts (timestamp) column and created a separate Date column for easier time-based analysis.

### Filtered Short Tracks:

- Removed rows where playback duration was ≤ 30 seconds. These are typically skipped songs that don't provide meaningful insights and would skew the results.

### Created a Calendar Table:

- Generated a calendar table with the following columns:
  - Year, Date, Month Name, Month (for sorting months), Week of Month, Weekdays, Weekday Sort (for sorting weekdays).

### Generated Unique Track Identifier (DAX):

- Created a calculated column in DAX to generate a unique_uri_track for tracks with the same title but different identifiers, ensuring accurate tracking of individual songs.

