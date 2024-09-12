# Claim vs opinion classification prediction project

## Overview

The goal of this project is to classify TikTok videos as either "claims" or "opinions" using machine learning models. By analyzing video engagement metrics and textual data from video transcripts, the project aims to improve the efficiency of content moderation on the platform.

## Dataset

The dataset used for this project includes the following features:

- **claim_status**: Binary label indicating if a video is a claim or an opinion.
- **video_id**: Unique identifier for each video.
- **video_duration_sec**: Duration of the video in seconds.
- **video_transcription_text**: Transcription of the video's audio.
- **verified_status**: Whether the author of the video is verified (categorical).
- **author_ban_status**: Whether the author is banned (categorical).
- **video_view_count**: Number of views the video has received.
- **video_like_count**: Number of likes the video has received.
- **video_share_count**: Number of shares the video has received.
- **video_download_count**: Number of downloads the video has received.
- **video_comment_count**: Number of comments on the video.

## Techniques Used

- **Feature Engineering**: Created and transformed features to enhance model performance, including converting categorical variables and text data into numeric features.
- **Data Preprocessing**: Cleaned and prepared the data, handling missing values and encoding categorical variables.
- **Modeling**: Implemented and compared various machine learning models for classification.

## Algorithms Used

- **Random Forest**: An ensemble method that uses multiple decision trees to improve prediction accuracy.
- **XGBoost**: An advanced ensemble technique that builds models sequentially to correct the errors of previous models.

## Results

- **Best Model**: Random Forest
- **Performance Metric**: Achieved a Recall Score of 0.995 on the test dataset, indicating high effectiveness in identifying claims.
- **Feature Importance**: Video engagement metrics (e.g., view count, like count) were the most influential features in predicting claim status.

## Conclusion

The Random Forest model demonstrated excellent performance with a high recall score, effectively identifying videos that are likely to be claims. The analysis revealed that video engagement levels are critical predictors of claim status.

## Future Plans

- **Model Improvement**: Explore additional features and advanced techniques to further enhance model accuracy.
- **Data Collection**: Gather more data to improve model robustness and accuracy.
- **Feature Engineering**: Refine and select features to improve model performance.
- **Model Deployment**: Consider deploying the model in a real-world scenario and establish monitoring practices.
- **Exploratory Data Analysis (EDA)**: Conduct further EDA to gain deeper insights and optimize feature selection.
