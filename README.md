# Stoicism-Related-Tweets-Key-Findings-and-Insights

## Overview

This repository contains the analysis of geotagged tweets related to Stoicism from 2010 to July 2023, sourced from the **Geotweet Archive v2.0** (Harvard CGA). The project aims to investigate the public discourse surrounding Stoicism on Twitter, focusing on sentiment distribution, geographical distribution, temporal trends, and the resolution of previously categorized "Unknown" tweets. The analysis also explores correlations between tweet volume and sentiment and maps the geographical distribution of Stoicism-related tweets across the globe.

## Key Findings

- **Sentiment Distribution:** 49% of the tweets express positive sentiment, 35% neutral, and 16% negative.
- **Geographical Distribution:** High tweet volumes are observed in English-speaking countries such as the United States, United Kingdom, and South Africa. Bermuda and the Bahamas showed notable engagement in Stoic discussions.
- **Temporal Trends:** A peak in positive sentiment occurred in 2014, with a gradual decline in positivity over time.
- **Correlation between Tweet Volume and Sentiment:** A weak negative correlation of -0.18 was found, indicating that sentiment is not strongly influenced by tweet volume.
- **Unknown Tweets Resolution:** "Unknown" tweets were mapped to specific countries using geographical coordinates, resolving their locations to countries like the United States, Bermuda, and the United Kingdom.

## Data

- **Source:** Geotweet Archive v2.0 (Harvard CGA)
- **Period:** 2010–July 2023
- **Metrics Analyzed:**
  - Tweet Volume
  - Sentiment Polarity (Positive, Neutral, Negative)
  - Geographical Distribution (Latitude, Longitude)

### Data Access

The data used for this analysis can be accessed through the [Geotweet Archive v2.0](https://doi.org/doi:10.7910/DVN/3NCMB6) or by accessing the raw tweet data files provided in the repository.

### Geospatial Coordinates Data

The country coordinates used to map the "Unknown" tweets can be accessed via this [GitHub raw file](https://gist.githubusercontent.com/metal3d/5b925077e66194551df949de64e910f6/raw/c5f20a037409d96958553e2eb6b8251265c6fd63/country-coord.csv).

## Methodology

The methodology follows these key steps:

1. **Data Preprocessing:** Tweets were filtered to include only those containing Stoicism-related keywords. The dataset was cleaned, and sentiment analysis was applied to classify tweets as positive, neutral, or negative.
2. **Geospatial Mapping:** Geospatial coordinates (latitude and longitude) were used to map tweets' geographical origins. "Unknown" tweets, previously unclassified, were resolved using the country coordinates data from the GitHub raw file.
3. **Sentiment Analysis:** Tweets were classified based on sentiment polarity, and the sentiment distribution was analyzed over time.
4. **Geographical and Temporal Trends:** Heatmaps and graphs were generated to visualize the geographical distribution and sentiment trends over time.

## Visualizations

The following visualizations were generated as part of the analysis:

- **Figure 1:** Sentiment Distribution of Stoicism-Related Tweets (Pie chart showing positive, neutral, and negative sentiment)
- **Figure 2:** Heatmap of Stoicism-Related Tweets by Region (Interactive heatmap of tweet volume across the world, zoomed into Cambridge/Boston area for local engagement)
- **Figure 3:** Temporal Trends in Sentiment of Stoicism-Related Tweets (Line chart showing sentiment shifts over time)
- **Figure 4:** Mapping of 'Unknown' Tweets to Country Locations (Geospatial map showing how 'Unknown' tweets were mapped to countries)

The interactive heatmap and other charts are saved as `.html` files and `.png` images in the repository for reference.

## Installation

To run this analysis on your own machine, follow these steps:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/stoicism-tweet-analysis.git
2. Install required dependencies: Ensure you have Python 3.8 or higher installed and set up a virtual environment. Then, install the necessary libraries:
  !pip install -r requirements.txt
   
3. Run the notebook: Start Jupyter Notebook and open the analysis file:
jupyter notebook Stoicism_Tweet_Analysis.ipynb


Future Work
Negative Sentiment Analysis: Further investigation into the specific triggers or controversies influencing negative discussions of Stoicism.

Sentiment Shifts with Events: Cross-referencing sentiment trends with external events, such as public figures' endorsements or specific movements, could provide a more nuanced understanding of shifts in Stoic discourse.

Authors
Rafael Albuquerque (Visiting Scholar, Harvard CGA)
Devika Kakkar (Harvard CGA)

License
This project is licensed under the Harvard CGA terms, and the content derived from the Geotweet Archive is subject to its respective terms of use.

