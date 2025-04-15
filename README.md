# 🧠 Stoicism on Twitter — A Geospatial & Sentiment Analysis (2010–2023)

Welcome to the official repository of our large-scale analysis of Stoicism-related discourse on Twitter 🌍. This project explores **how, where, and with what sentiment** Stoic ideas were shared over more than a decade — using advanced geospatial tools, sentiment modeling, and interactive maps. 

Built during a research residency at **Harvard CGA** by  
**Rafael Albuquerque** & **Devika Kakkar**.

---

## 📦 Project Overview

- **🗓️ Timeframe:** Jan 2010 to July 2023  
- **🧵 Dataset:** [Geotweet Archive v2.0](https://doi.org/10.7910/DVN/3NCMB6) — 10B+ tweets  
- **🧭 Focus:** Sentiment polarity, geolocation, temporal shifts  
- **🧮 Total Tweets Analyzed:** `678,498`  
- **📍 Geolocated:** Yes — tweets contain latitude & longitude  
- **🧪 Method:** NLP + Geospatial + Exploratory Visualization  
- **🌐 Notebook-Friendly:** All code written for Jupyter notebooks with full outputs  

---

## 🔍 Key Findings

| Metric | Value |
|--------|-------|
| 😊 Positive Sentiment | **49%** |
| 😐 Neutral Sentiment | **35%** |
| 😠 Negative Sentiment | **16%** |
| 🌎 Top Country | **United States** (235K+ tweets) |
| 📉 Correlation Volume x Sentiment | `r = -0.18` (p = 0.07128) |
| 🧭 "Unknown" Tweets Resolved | Mapped to **233 countries** using coordinates |

> 🔁 See `/figures/` for all outputs including maps and charts.

---

## 📊 Visualizations

| 🔢 Figure | 📍 Location | 🖼️ Description |
|----------|-------------|----------------|
| **Figure 1** | Block 2B | Sentiment Pie Chart |
| **Figure 2** | Block 2F | Interactive Heatmap of Stoic Tweets |
| **Figure 3** | Block 2G | Temporal Line Chart of Sentiment Over Time |
| **Figure 4** | Block 2H | Scatter Plot: Tweet Volume × Sentiment |
| **Figure 5** | Block 2I | Resolution of Unknown Tweets by Coordinates |
| **Figure 6** | Block 2J | Country-Level Sentiment Table |

> 📌 **Tip**: You can open `Figure 2` in any browser and zoom into Cambridge, MA or your region of interest.

---

## ⚙️ How to Run

bash
# 1. Clone the repo
git clone https://github.com/youruser/stoicism-twitter-analysis.git

# 2. Create a virtual environment and install dependencies
pip install -r requirements.txt

# 3. Run the Jupyter notebook
jupyter notebook Stoicism_Tweet_Analysis.ipynb```



💡 Use Python 3.8+. Compatible with HPC environments and supports multiprocessing (64 cores, 990GB RAM, 4 GPUs setup tested).


🧠 Methodology
Keyword Filtering:
Tweets were filtered using a curated list of Stoic roots and terms like stoic*, seneca, amorfati, mementomori, etc. Regex logic handled partial matches.

Sentiment Analysis:
We used pre-trained transformer-based models to label sentiment per tweet (positive, neutral, negative).

Geolocation:

Tweets with coordinates were directly mapped

"Unknown" locations were resolved using country centroid distances

Temporal Analysis:
Sentiment was tracked by year and visualized in time series plots.

Volume–Sentiment Correlation:
Pearson correlation tested between tweet volume and average sentiment per month.

📚 Citations
Lewis, Benjamin, and Devika Kakkar. 2016. “Harvard CGA Geotweet Archive v2.0.” Harvard Dataverse. https://doi.org/10.7910/DVN/3NCMB6

👥 Authors
Rafael Albuquerque
Visiting Scholar – Harvard CGA
PhD Candidate in Marketing @ UFRGS

Devika Kakkar
Senior Researcher – Harvard CGA
Creator of Geotweet Archive




🌟 Acknowledgments
This research was made possible thanks to:
Harvard CGA computing infrastructure
The open-source Python NLP and geospatial community




🚀 Ready to Explore?
Check the notebook Stoicism_Tweet_Analysis.ipynb and dive into the philosophy-powered Twitterverse 🌌
