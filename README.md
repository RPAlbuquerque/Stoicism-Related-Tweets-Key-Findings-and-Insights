# 🧠 Stoicism on Twitter — A Geospatial Analysis (2010–2023)

Welcome to the official repository of our large-scale analysis of Stoicism-related discourse on Twitter 🌍. This project explores how, where, and with what intensity Stoic ideas circulated globally over more than a decade — using advanced geospatial tools, semantic validation, and interactive maps.

Built during a research residency at Harvard CGA by  
**Rafael Albuquerque & Devika Kakkar**

---

## 📦 Project Overview

| Metric                           | Value                                  |
|----------------------------------|----------------------------------------|
| 🗓️ Timeframe                     | Jan 2010 to July 2023                  |
| 🧵 Dataset                       | Geotweet Archive v2.0 (10B+ tweets)    |
| 🧮 Tweets with Stoic Terms       | 23.3 million (initial keyword match)   |
| 🧠 Semantically Validated Tweets | **1.73 million**                       |
| 📍 Geolocated                    | 100% (mapped to 150+ countries)        |
| 🧪 Method                        | Regex + Semantic Filtering + KDTree    |
| ⚙️ Performance                   | Multiprocessing on 64 cores, 990GB RAM |
| 📁 Notebook-Compatible           | All steps run via Jupyter (Python 3.8+) |

---

## 🔍 Key Findings

| Insight                      | Result                                |
|-----------------------------|----------------------------------------|
| 🌎 Top Country              | United States (473,000+ tweets)        |
| 📌 Most Frequent Term       | `stoic`, followed by `philosoph`, `seneca` |
| 🔀 Cluster Outliers         | Bermuda, Bahamas, Saudi Arabia         |
| 🧠 Conceptual Distinctions  | Modern usage (`mementomori`, `stoic`) vs. classical (`seneca`, `plato`) |
| 🗺️ Mapping Success          | 100% of tweets assigned to countries   |
| 📊 Longitudinal Coverage    | 2011–2023 (semantic validity from 2011) |

---

## 📊 Visualizations

| 🔢 Figure | 📍 Location                          | 🖼️ Description                                       |
|----------|--------------------------------------|------------------------------------------------------|
| Fig. 1   | `plots/term_evolution.png`           | Temporal evolution of Stoicism-related terms         |
| Fig. 2   | `plots/top10_total_terms_by_country.png` | Top 10 countries by total mentions                |
| Fig. 3   | `plots/stacked_top_terms_by_country.png` | Distribution of top terms by country              |
| Fig. 4   | `plots/semantic_clusters_countries.png`  | PCA + KMeans clustering of countries by term usage |
| Fig. 5   | `stoicism_heatmap_global.html`       | Interactive dark-mode map of geolocated tweets       |
| Fig. 6   | `stoicism_heatmap_global_light.html` | Interactive light-mode version of the map            |

📌 **Tip:** You can open the interactive heatmaps in any browser and zoom into your region of interest.

---

## ⚙️ How to Run

```bash
# 1. Clone the repo
git clone https://github.com/youruser/stoicism-twitter-analysis.git

# 2. Create a virtual environment and install dependencies
pip install -r requirements.txt

# 3. Launch the notebook
jupyter notebook Stoicism_Tweet_Analysis.ipynb

🧠 Methodology
🔍 Keyword Filtering
Tweets were filtered using a curated list of 60+ Stoic-related roots and terms (e.g., stoic*, seneca, amorfati, mementomori) with word-boundary-aware regex logic.

🧠 Semantic Validation
To eliminate false positives, each keyword match was re-verified in context. Only tweets where the term was conceptually valid were retained (e.g., excluding "stoic cat").

🌐 Geolocation
Tweets were mapped to countries using:

Native GPS coordinates (lat/lon)

KDTree nearest-neighbor mapping to 150+ country centroids

🕰️ Temporal Analysis
Valid tweets were aggregated by year and term, enabling trend analysis across 2011–2023.

📈 Clustering
A PCA + KMeans approach was used to cluster countries by term usage patterns, revealing cultural groupings and outliers.

📚 Citation
Lewis, Benjamin, and Devika Kakkar. 2016.
“Harvard CGA Geotweet Archive v2.0.” Harvard Dataverse.
https://doi.org/10.7910/DVN/3NCMB6

👥 Authors
Rafael Pereira de Albuquerque
Visiting Scholar – Harvard CGA
PhD Candidate in Marketing @ UFRGS
rafaelpereiraalbuquerque@fas.harvard.edu

Devika Kakkar
GIS Data Science Project Manager – Harvard CGA
Creator of Geotweet Archive



🌟 Acknowledgments
This research was made possible thanks to:

Harvard CGA computing infrastructure

The open-source Python NLP + GIS community

Professors and collaborators supporting Stoicism v3

🚀 Ready to Explore?
Check the notebook Stoicism_Tweet_Analysis.ipynb
and dive into the philosophy-powered Twitterverse 🌌
