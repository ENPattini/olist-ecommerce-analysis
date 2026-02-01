# Olist Brazilian E-Commerce Analytics

*Available in: 🇬🇧 English (this file) | 🇪🇸 Español → [README.es.md](README.es.md) | 🇮🇹 Italiano → [README.it.md](README.it.md)*

![Python](https://img.shields.io/badge/python-3.11-blue)
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)

End-to-end business analysis of the public Olist dataset (~100k orders, 2016–2018).  

Focus: actionable insights on sales trends, customer segmentation (RFM), cohort retention, delivery performance, and revenue forecasting with Prophet.



### Tech Stack

- Python: pandas, numpy, seaborn, plotly, prophet
- Visualization: Plotly (interactive)
- Dashboard: Power BI
- Reproducibility: conda environment.yml


### Interactive Dashboard & Report

- **Interactive HTML Report**: 

    [View Olist Analysis Report (HTML)](https://emilionahuelpattini.com/en/data/data-analysis/projects/olist-report/olist-ecommerce-analysis.html)  


- **Power BI Dashboard** (recommended – full interactivity):

    [Open in Power BI Service](https://app.powerbi.com/view?r=eyJrIjoiNTFjYTAyYTctYTU0YS00ZWIzLTljZTEtMDQ0MjA4MzljODI3IiwidCI6IjZiNTQyOWEzLTM3MjItNDA3Yy04NmQyLWY4MGViNjEwMjU4MSIsImMiOjR9)


- **Download PDF Version** (print-friendly – English):  

    [Download Olist Analysis Report – PDF](report/Olist-Ecommerce-Analysis-EN.pdf)


### Highlights

- RFM segmentation: 97% one-time buyers, Champions drive disproportionate revenue
- Cohort retention: Month 1 only ~0.3–0.7% → massive retention opportunity
- Revenue concentration: SP ~60%, top 5 categories ~40–50%
- Delivery performance: average ~12 days earlier than estimated, with regional variation
- Forecast 2019: moderate growth ~600k–900k BRL/month with subtle seasonal peaks


### Repository Structure

```
Olist-Ecommerce-Analysis/
├── Olist-Ecommerce-Analysis-EN.ipynb     # English (main notebook)
├── Olist-Ecommerce-Analysis-ES.ipynb     # Spanish version
├── Olist-Ecommerce-Analysis-IT.ipynb     # Italian version
├── README.md                             # English | -IT | -ES versions
├── environment.yml                       # Conda environment
├── .gitignore
├── data/
│   └── processed/                        # Exported CSVs
├── dashboard/
│   └── Olist_Analytics_Dashboard.pbix    # Power BI file
├── report/
│   ├── Olist-Ecommerce-Analysis-static.html  # Static HTML exports (EN|IT|ES)
│   └── Olist-Ecommerce-Analysis.pdf          # PDF export (EN|IT|ES)
└── images/screenshots                   # Dashboard & notebook screenshots
```

### How to Run

1. Clone the repository:
```
git clone https://github.com/yourusername/Olist-Ecommerce-Analysis.git

cd Olist-Ecommerce-Analysis
```

2. **Download the dataset** (required – not included in repo due to size):

    - Original raw Olist dataset: [Download from Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce) (~300 MB)  
    - Extract it to `./data/raw/` (create the folder if needed)  
    - The notebook expects the raw files in `./data/raw/` and processes them to `./data/processed/`


3. Create and activate the environment:

```
conda env create -f environment.yml

conda activate olist
```

4. Launch Jupyter Lab:

```
jupyter lab
```

5. Open any of the notebooks (EN/ES/IT) and run all cells.


### Screenshots

**Olist Overview Page** 

![*Global KPIs, forecast, cohort heatmap, RFM bar, state bubble map, top categories*](images/screenshots/olist_overview_page.png)  


**Customer Deep Dive Page**

![*RFM scatter, filtered customer table, segment KPIs & Gauges*](images/screenshots/customer_deep_dive_page.png)



### Lessons Learned & Next Steps

- Python transition from R successful: pandas for data manipulation, Prophet for forecasting, Plotly for interactive plots, Power BI for dashboarding
- E-commerce reality: extremely low repeat rates (~3%) require strong retention focus
- Importance of business context: every analysis led to concrete recommendations
- Future: Streamlit app, A/B testing retention tactics, external data integration



### Contact

- 📧 contact@emilionahuelpattini.com

- 💼 https://www.linkedin.com/in/emilionahuelpattini

- 🐙 https://github.com/ENPattini

Thanks for taking a look!

Feedback welcome — open an issue or reach out!

© 2026 Emilio Nahuel Pattini



**License**

This project is licensed under the MIT License – see the [LICENSE](LICENSE) file for details.
