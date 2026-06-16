<div align="center">

# 📊 Google Search Analysis

### Exploratory Data Analysis of Google Search Behavior using Search Console API & PyTrends

[![Python](https://img.shields.io/badge/Python-3.9%2B-blue?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)

</div>

---

## 🔍 Overview

This project performs a deep-dive exploratory data analysis (EDA) on Google Search data by combining two powerful data sources:

- **Google Search Console API** — Real search performance metrics (clicks, impressions, CTR, position)
- **PyTrends (Google Trends API)** — Keyword popularity trends, related queries, and rising search terms

The goal is to uncover actionable SEO insights, identify traffic patterns, and understand how user search behavior evolves over time — useful for **SEO strategists, digital marketers, and data analysts**.

---

## 🗂️ Project Structure

```
Google-Search-Analysis/
│
├── 📓 Google Data Analysis Through Their Api.ipynb   # Main analysis notebook
├── 📄 data-export (1).csv                            # Dataset from Google Search Console
├── 📋 requirements.txt                               # Project dependencies
└── 📝 README.md                                      # Project documentation
```

---

## 📌 Key Features

| Feature | Description |
|---|---|
| 🔑 **Keyword Performance** | Analyze top queries by clicks, impressions, and average position |
| 📈 **CTR Analysis** | Identify high-impression but low-CTR keywords (optimization opportunities) |
| 🌍 **Country-wise Traffic** | Breakdown of search traffic by geographic region |
| 📱 **Device Distribution** | Desktop vs. Mobile vs. Tablet usage patterns |
| 📅 **Trend Over Time** | Track search interest and performance across date ranges |
| 🔥 **Rising Keywords** | Discover trending and breakout search terms via PyTrends |
| 🔗 **Related Queries** | Surface semantically related search terms |
| 📊 **Page-level Insights** | Identify top-performing landing pages from organic search |

---

## 📊 Visualizations Included

- **CTR vs. Impressions** — Scatter plot to identify quick-win keywords
- **Clicks Over Time** — Line chart showing traffic trends
- **Country-wise Performance** — Bar chart of traffic by region
- **Query Frequency** — Bar plot of top search queries
- **Device Usage** — Pie chart of device distribution
- **Correlation Heatmap** — Relationships between search metrics

---

## 🧹 Data Processing Pipeline

```
Raw GSC Export (.csv)
        ↓
  Data Cleaning
  ├── Remove null/invalid entries
  ├── Normalize keyword strings
  ├── Convert dates to datetime
  └── Filter low-volume noise
        ↓
  Feature Engineering
  ├── Group by country / device / page
  ├── Calculate CTR buckets
  └── Merge with PyTrends data
        ↓
  EDA & Visualization
        ↓
  Insights & Reporting
```

---

## 📁 Dataset

The dataset (`data-export.csv`) is exported directly from **Google Search Console** and contains the following columns:

| Column | Description |
|---|---|
| `query` | Search keyword/phrase |
| `clicks` | Number of clicks from search results |
| `impressions` | How many times the page appeared in search |
| `ctr` | Click-through rate (clicks / impressions) |
| `position` | Average ranking position in Google |
| `country` | User's country |
| `device` | Device type (desktop / mobile / tablet) |
| `date` | Date of the search data |

---

## ⚙️ Tech Stack

| Tool | Purpose |
|---|---|
| `Python 3.9+` | Core programming language |
| `Pandas` | Data manipulation and analysis |
| `NumPy` | Numerical operations |
| `Matplotlib` | Static visualizations |
| `Seaborn` | Statistical data visualization |
| `PyTrends` | Google Trends API wrapper |
| `Google Search Console API` | Real-time search performance data |
| `Jupyter Notebook` | Interactive analysis environment |

---

## 🚀 Getting Started

### Prerequisites

```bash
Python 3.9+
pip
```

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/Amankhan0087/Google-Search-Analysis.git
cd Google-Search-Analysis

# 2. Install dependencies
pip install -r requirements.txt

# 3. Launch Jupyter Notebook
jupyter notebook "Google Data Analysis Through Their Api.ipynb"
```

### requirements.txt

```
pandas
numpy
matplotlib
seaborn
pytrends
google-auth
google-auth-oauthlib
google-auth-httplib2
google-api-python-client
jupyter
```

---

## 💡 Key Insights Extracted

- ✅ Which search queries generate the **most clicks vs. impressions**
- ✅ Pages with **high impressions but poor CTR** (title/meta optimization needed)
- ✅ **Top-performing landing pages** from organic search
- ✅ Countries generating **maximum organic traffic**
- ✅ **Device split** — how users reach you (mobile vs. desktop dominant)
- ✅ **Peak traffic days/dates** for content publishing strategy
- ✅ **Rising keyword trends** to capitalize on before competition increases

---

## 🔭 Future Roadmap

- [ ] 🖥️ Build an interactive **SEO Dashboard** (Streamlit or Power BI)
- [ ] 📉 Add **time-series forecasting** using Prophet / ARIMA
- [ ] 🧠 Implement **keyword clustering** using NLP (TF-IDF / K-Means)
- [ ] ☁️ Scale to large datasets using **Google BigQuery**
- [ ] 📬 Automate weekly **email reports** with key SEO metrics
- [ ] 🔄 Schedule **live data pulls** from GSC API via cron jobs

---

## 🤝 Contributing

Contributions are welcome! Here's how:

```bash
# 1. Fork the repo
# 2. Create your feature branch
git checkout -b feature/your-feature-name

# 3. Commit your changes
git commit -m "Add: your feature description"

# 4. Push to the branch
git push origin feature/your-feature-name

# 5. Open a Pull Request
```

For major changes, please open an **issue** first to discuss what you'd like to change.

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

## 👨‍💻 Author

<div align="center">

**Aman Khan**

*AI Engineer | Data Analyst | Python Developer*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/aman-khan-data-scientist/)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Amankhan0087)
[![Portfolio](https://img.shields.io/badge/Portfolio-Visit-FF5722?style=for-the-badge&logo=google-chrome&logoColor=white)](https://amankhan.online)

</div>

---

<div align="center">

⭐ **If you found this project useful, please consider giving it a star!** ⭐

</div>
