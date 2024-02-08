# youtube_api
This code uses Youtube API to scrape channel data 


### This is an api code for Alux Youtube Channel
# YouTube Channel Statistics and Analysis - Code Documentation

## Overview

This code documentation outlines the steps involved in fetching channel statistics, obtaining video details, and performing various analyses on the data. The analyses include transforming data types, calculating video duration in seconds, finding the best and least viewed episodes, creating visualizations such as violin plots and scatter plots, and generating word clouds.

### 1. Channel Statistics

#### 1.1. `get_channel_statistics(api_key, channel_id)`
Description:
Fetches basic statistics for the YouTube channel.
Parameters:
- `api_key`: Your YouTube Data API key.
- `channel_id`: The unique identifier of the YouTube channel.

#### 1.2. `get_video_ids(api_key, channel_id)`

Description:
Retrieves the video IDs of all videos in the channel.
Parameters:
- `api_key`: Your YouTube Data API key.
- `channel_id`: The unique identifier of the YouTube channel.

### 2. Video Details
#### 2.1. `get_video_details(api_key, video_ids)`

Description:
Fetches detailed information for each video using the provided video IDs.
Parameters:
- `api_key`: Your YouTube Data API key.
- `video_ids`: List of video IDs obtained from `get_video_ids`.

### 3. Data Transformation
#### 3.1. `transform_data(data)`
Description:
Converts data types for better analysis, e.g., converting timestamps to datetime objects.
Parameters:
- `data`: DataFrame containing video details.

### 4. Video Duration in Seconds
#### 4.1. `get_duration_seconds(data)`
Description:
Calculates the duration of each video in seconds.
Parameters:
- `data`: DataFrame containing video details.

### 5. Best and Least Viewed Episodes
#### 5.1. `get_best_episode(data)`
Description:
Identifies the episode with the highest views.
Parameters:
- `data`: DataFrame containing video details.

#### 5.2. `get_least_episode(data)`
Description:
Identifies the episode with the least views.
Parameters
- `data`: DataFrame containing video details.

### 6. Visualization
#### 6.1. `plot_violin(data)`
Description:
Generates a violin plot to visualize the distribution of views for videos.
Parameters:
- `data`: DataFrame containing video details.

#### 6.2. `scatter_plot(data)`
Description:
Creates scatter plots of comments against views and likes against views.
Parameters:
- `data`: DataFrame containing video details.
#### 6.3. `plot_duration_vs_videos(data)`
Description:
Plots video duration against the number of videos.
Parameters:
- `data`: DataFrame containing video details.

### 7. Word Cloud Title
#### 7.1. `generate_word_cloud(data)`
Description:
Generates a word cloud based on video titles.
Parameters:
- `data`: DataFrame containing video details.

### 8. Most Published Days
#### 8.1. `most_published_days(data)`
Description:
Identifies the days on which the channel publishes the most episodes.
Parameters:
- `data`: DataFrame containing video details.

### 9. Word Count on Comments
#### 9.1. `generate_word_cloud(data)`
Description:
Generates a word cloud based on video comments.
Parameters:
- `data`: DataFrame containing video details.

### 10. Data Frame of Comments

#### 10.1. `create_comments_dataframe(data)`
Description:
Creates a DataFrame specifically for video comments.
Parameters:
- `data`: DataFrame containing video details.

## Conclusion

This code documentation serves as a guide for analyzing YouTube channel statistics, obtaining video details, and performing various insightful analyses using Python. Each function is designed to perform specific tasks, facilitating a comprehensive analysis of the channel's content and engagement.
generate_word_cloud(data)¶
Description: Generates a word cloud based on video titles. Parameters:

data: DataFrame containing video details.
Credits: Thu Vu on youtube.
