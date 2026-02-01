# Analisi dell'E-Commerce Brasiliano – Olist

*Disponibile in: 🇬🇧 English → [README.md](README.md) | 🇪🇸 Español → [README.es.md](README.es.md) | 🇮🇹 Italiano (questo file)*

![Python](https://img.shields.io/badge/python-3.11-blue)
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)

Analisi end-to-end orientata al business del dataset pubblico Olist (~100k ordini, 2016–2018).

Focus: insight actionable su trend di vendite, segmentazione clienti (RFM), retention dei cohorts, performance di consegna e previsione dei ricavi con Prophet.


### Tech Stack

- Python: pandas, numpy, seaborn, plotly, prophet
- Visualizzazione: Plotly (interattivo)
- Dashboard: Power BI
- Riproducibilità: conda environment.yml


### Dashboard e Report Interattivi

- **Report HTML Interattivo**: 

    [Visualizza Olist Analysis Report (HTML)](https://emilionahuelpattini.com/it/data/data-analysis/projects/olist-report/olist-ecommerce-analysis.html)  


- **Dashboard Power BI** (raccomandato – piena interattività):

    [Apri in Power BI Service](https://app.powerbi.com/view?r=eyJrIjoiNTFjYTAyYTctYTU0YS00ZWIzLTljZTEtMDQ0MjA4MzljODI3IiwidCI6IjZiNTQyOWEzLTM3MjItNDA3Yy04NmQyLWY4MGViNjEwMjU4MSIsImMiOjR9)


- **Scarica Versione PDF** (stampabile):   

    [Scarica Olist Analysis Report – PDF](report/Olist-Ecommerce-Analysis-IT.pdf)


### Punti salienti

- Segmentazione RFM: 97% clienti one-time, Champions generano ricavi sproporzionati
- Retention dei cohorts: Mese 1 solo ~0.3–0.7% → enorme opportunità in strategie post-acquisto
- Concentrazione ricavi: SP ~60%, top 5 categorie ~40–50%
- Performance di consegna: media ~12 giorni prima del previsto, con variazione regionale
- Previsione 2019: crescita moderata ~600k–900k BRL/mese con picchi stagionali sottili


### Struttura del Repository

```
Olist-Ecommerce-Analysis/
├── Olist-Ecommerce-Analysis-EN.ipynb         # Inglese (notebook principale)
├── Olist-Ecommerce-Analysis-ES.ipynb         # Versione spagnola
├── Olist-Ecommerce-Analysis-IT.ipynb         # Versione italiana
├── README.md # Inglese | -IT | -ES versioni
├── environment.yml                           # Ambiente conda
├── .gitignore
├── data/
│ └── processed/                              # CSVs esportati
├── dashboard/
│ └── Olist_Analytics_Dashboard.pbix          # File Power BI
├── report/
│ ├── Olist-Ecommerce-Analysis-static.html    # Exports HTML statici (EN|IT|ES)
│ └── Olist-Ecommerce-Analysis.pdf            # Export PDF (EN|IT|ES)
└── images/screenshots                    # Screenshot del dashboard e notebook
```

### Come Eseguire

1. Clona il repository:

```
git clone https://github.com/yourusername/Olist-Ecommerce-Analysis.git

cd Olist-Ecommerce-Analysis
```

2. **Scaricare il dataset** (richiesto – non incluso nel repo per dimensioni):  

    - Dataset originale raw Olist: [Scarica da Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce) (~300 MB)  
    - Estrarlo in `./data/raw/` (crea la cartella se necessario)  
    - Il notebook si aspetta i file raw in `./data/raw/` e li processa in `./data/processed/`
    

3. Crea e attiva l'ambiente:

```
conda env create -f environment.yml

conda activate olist
```

4. Avvia Jupyter Lab:

```
jupyter lab
```

5. Apri uno qualsiasi dei notebook (EN/ES/IT) ed esegui tutte le celle.


### Screenshots

**Pagina Olist Overview** 

![*KPI globali, linea previsione, heatmap cohorts, barra RFM, mappa bubble per stato, top categorie*](images/screenshots/olist_overview_page.png)  


**Pagina Customer Deep Dive**

![*Scatter RFM, tabella clienti filtrata, KPI e Gauges per segmento*](images/screenshots/customer_deep_dive_page.png)



### Lezioni Apprese e Prossimi Passi

- Transizione riuscita da R a Python: pandas per manipolazione dati, Prophet per forecasting, Plotly per visual interattivi, Power BI per dashboarding
- Realtà dell'e-commerce: tassi di ripetizione estremamente bassi (~3%) richiedono forte focus sulla retention
- Importanza del contesto business: ogni analisi ha portato a raccomandazioni concrete
- Futuro: app Streamlit, A/B testing su tattiche di retention, integrazione dati esterni



### Contatti

- 📧 contact@emilionahuelpattini.com

- 💼 https://www.linkedin.com/in/emilionahuelpattini

- 🐙 https://github.com/ENPattini

Grazie per aver dato un'occhiata!  

Feedback benvenuto — apri un issue o scrivimi.

© 2026 Emilio Nahuel Pattini



**Licenza**

Questo progetto è licenziato sotto la Licenza MIT – vedi il file [LICENSE](LICENSE) per dettagli.
