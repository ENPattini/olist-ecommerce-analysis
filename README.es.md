# Análisis de E-Commerce Brasileño – Olist

*Disponible en: 🇬🇧 English → [README.md](README.md) | 🇪🇸 Español (este archivo) | 🇮🇹 Italiano → [README.it.md](README.it.md)*

![Python](https://img.shields.io/badge/python-3.11-blue)
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)

Análisis end-to-end orientado al negocio del dataset público de Olist (~100k órdenes, 2016–2018).  

Enfoque: insights accionables sobre tendencias de ventas, segmentación de clientes (RFM), retención de cohorts, performance de entrega y pronóstico de ingresos con Prophet.



### Tech Stack

- Python: pandas, numpy, seaborn, plotly, prophet
- Visualización: Plotly (interactivo)
- Dashboard: Power BI
- Reproducibilidad: conda environment.yml


### Dashboard y Reporte Interactivos

- **Reporte HTML Interactivo**:  

  [Ver Olist Analysis Report (HTML)](https://emilionahuelpattini.com/es/data/data-analysis/projects/olist-report/olist-ecommerce-analysis.html)

- **Dashboard en Power BI** (recomendado – interactividad completa): 

  [Abrir en Power BI Service](https://app.powerbi.com/view?r=eyJrIjoiNTFjYTAyYTctYTU0YS00ZWIzLTljZTEtMDQ0MjA4MzljODI3IiwidCI6IjZiNTQyOWEzLTM3MjItNDA3Yy04NmQyLWY4MGViNjEwMjU4MSIsImMiOjR9)

- **Descargar Versión PDF** (para impresión):  

  [Descargar Olist Analysis Report – PDF](report/Olist-Ecommerce-Analysis-ES.pdf)



### Highlights

- Segmentación RFM: 97% clientes one-time, Champions generan revenue desproporcionado
- Retención de cohorts: Mes 1 solo ~0.3–0.7% → enorme oportunidad en estrategias post-compra
- Concentración de ingresos: SP ~60%, top 5 categorías ~40–50%
- Performance de entrega: promedio ~12 días antes de lo estimado, con variación regional
- Pronóstico 2019: crecimiento moderado ~600k–900k BRL/mes con picos estacionales sutiles


### Estructura del Repositorio

```
Olist-Ecommerce-Analysis/
├── Olist-Ecommerce-Analysis-EN.ipynb     # English Inglés (notebook principal)
├── Olist-Ecommerce-Analysis-ES.ipynb     # Versión en español
├── Olist-Ecommerce-Analysis-IT.ipynb     # Versión en italiano
├── README.md                             # Inglés | -IT | -ES versiones
├── environment.yml                       # Entorno conda
├── .gitignore
├── data/
│   └── processed/                        # CSVs exportados
├── dashboard/
│   └── Olist_Analytics_Dashboard.pbix    # Archivo Power BI
├── report/
│   ├── Olist-Ecommerce-Analysis-static.html  # Exports HTML estáticos (EN|IT|ES)
│   └── Olist-Ecommerce-Analysis.pdf          # Export PDF (EN|IT|ES)
└── images/screenshots                   # Capturas del dashboard
```

### Cómo Ejecutar

1. Clonar el repositorio:

```
git clone https://github.com/yourusername/Olist-Ecommerce-Analysis.git

cd Olist-Ecommerce-Analysis
```

2. **Descargar el dataset** (requerido – no incluido en el repo por tamaño):  

    - Dataset original raw de Olist: [Descargar desde Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce) (~300 MB)  
    - Extraerlo en `./data/raw/` (crear la carpeta si es necesario)  
    - El notebook espera los archivos raw en `./data/raw/` y los procesa a `./data/processed/`
    

3. Crear y activar el entorno:

```
conda env create -f environment.yml

conda activate olist
```

4. Ejecutar Jupyter Lab:

```
jupyter lab
```

5. Abrir cualquiera de los notebooks (EN/ES/IT) y ejecutar todas las celdas.


### Capturas de Pantalla

**Página Olist Overview** 

![*KPIs globales, línea de pronóstico, heatmap de cohorts, barra RFM, mapa bubble por estado, top categorías*](images/screenshots/olist_overview_page.png)  


**Página Customer Deep Dive**

![*Scatter RFM, tabla de clientes filtrada, KPIs y Gauges por segmento*](images/screenshots/customer_deep_dive_page.png)



### Lecciones Aprendidas y Próximos Pasos

- Transición exitosa de R a Python: pandas para manipulación de datos, Prophet para forecasting, Plotly para visuales interactivos, Power BI para dashboarding
- Realidad del e-commerce: tasas de recompra extremadamente bajas (~3%) requieren fuerte foco en retención
- Importancia del contexto business: cada análisis llevó a recomendaciones concretas
- Futuro: app Streamlit, A/B testing de tácticas de retención, integración de datos externos



### Contacto

- 📧 contact@emilionahuelpattini.com

- 💼 https://www.linkedin.com/in/emilionahuelpattini

- 🐙 https://github.com/ENPattini

¡Gracias por echar un vistazo!  

Feedback bienvenido — abrí un issue o escribime.

© 2026 Emilio Nahuel Pattini



**Licencia**

Este proyecto está licenciado bajo la Licencia MIT – ver el archivo [LICENSE](LICENSE) para detalles.
