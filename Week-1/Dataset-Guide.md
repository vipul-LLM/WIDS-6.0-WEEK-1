# Dataset guide
Use the [Spotify Tracks Dataset](https://huggingface.co/datasets/maharshipandya/spotify-tracks-dataset) or its [Kaggle listing](https://www.kaggle.com/datasets/maharshipandya/-spotify-tracks-dataset). Download the CSV from the source and name it dataset.csv. Review source terms before using or redistributing it; this repository does not redistribute the dataset.

The dataset contains track metadata and precomputed audio features. Inspect actual columns rather than assuming every field is present.

| Feature | Interpretation |
|---|---|
| track_id | Track identifier; may recur across genres |
| track_name / artists | Track metadata |
| track_genre | Genre label |
| valence | Musical positivity proxy |
| energy | Perceived intensity proxy |
| danceability | Suitability for dancing |
| acousticness | Confidence that the track is acoustic |
| instrumentalness | Estimate of absence of vocals |
| tempo | Beats per minute |
| loudness | Overall loudness in decibels |
| popularity | Source-specific popularity score |

Check missing values, duplicate IDs, feature ranges and metadata inconsistencies. Repeated tracks may represent different genre labels; do not discard them without considering this. The dataset does not establish listener mood or contain user interaction history. Do not infer causation from correlations. Use only metadata and numerical features; no audio files or streaming access are required. If the source download is unavailable, ask the mentor for an appropriately licensed substitute with comparable features.
