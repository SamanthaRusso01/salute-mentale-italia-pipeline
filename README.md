# 🧠 Salute Mentale in Italia — Analisi del Sistema SISM 2024

> **Portfolio Project · Junior Data Analyst**  
> Stack: `SQL` · `Python` · `Power BI`

---

## Contesto del Progetto

Il **Sistema Informativo per la Salute Mentale (SISM)** raccoglie annualmente i dati di tutte le strutture psichiatriche pubbliche italiane. Il report 2024 copre oltre **800.000 utenti** seguiti dai Dipartimenti di Salute Mentale (DSM) del SSN, con una granularità che permette analisi per regione, diagnosi, sesso e fascia d'età.

Questo progetto analizza i dati SISM per ***tracciare l'evoluzione della salute mentale in Italia***, studiando i divari geografici, demografici e di genere e valutando l'efficacia dei servizi territoriali. Il lavoro è strutturato in tre fasi tecniche progressive (SQL → Python → Power BI) per dimostrare la capacità di gestire l'intero ciclo di vita del dato.

---

## 🎯 Domande di Ricerca

Il progetto segue una progressione narrativa logica, dal profilo dell'utenza all'appropriatezza del sistema:

| # | Domanda | Focus |
|---|---------|-------|
| **Q1** | Chi sono gli utenti della salute mentale in Italia? | Profilo demografico per sesso, età, diagnosi |
| **Q2** | Dove viene intercettata la malattia mentale — e dove rimane invisibile? | Disparità regionali nei tassi di prevalenza/incidenza |
| **Q3** | Come è cambiata la domanda di salute mentale dal 2015 al 2024? | Trend temporale e impatto del COVID-19 |
| **Q4** | I pazienti ricevono un'assistenza continua o vengono persi nel percorso di cura? | Continuità assistenziale e abbandono del trattamento |
| **Q5** | Il sistema risponde in modo appropriato alla severità della patologia? | Appropriatezza del setting per gruppo diagnostico |

---

## Tech Stack & Competenze Dimostrate

- **Data Architecture & Cleaning:** `SQL` per la pulizia, la normalizzazione e la modellazione del database (Star Schema).
- **Advanced Analytics:** `Python` (`pandas`, `numpy`, `matplotlib`, `seaborn`, `scipy`) per l'EDA, i test statistici e lo studio dei trend storici.
- **Data Visualization & Storytelling:** `Power BI` (`DAX`, `Data Modeling`) per la creazione di una dashboard interattiva per stakeholder non tecnici.
- **Version Control:** `Git` e `GitHub` per la gestione del codice e della documentazione.

---

## 📁 Struttura della Repository

```
sism-2024-mental-health-italy/
│
├── data/
│   ├── raw/                  # File originali — non modificarti
│   └── processed/            # Output puliti
│
├── sql/
│   ├── 01_schema.sql
│   ├── 02_cleaning.sql
│   ├── 03_q1_demographics.sql
│   ├── 04_q2_regional.sql
│   ├── 05_q3_trends.sql
│   ├── 06_q4_continuity.sql
│   └── 07_q5_appropriateness.sql
│
├── notebooks/
│   ├── 01_EDA_overview.ipynb
│   ├── 02_q1_demographics.ipynb
│   ├── 03_q2_regional_disparities.ipynb
│   ├── 04_q3_covid_trend.ipynb
│   ├── 05_q4_continuity.ipynb
│   └── 06_q5_appropriateness.ipynb
│
├── powerbi/
│   └── SISM_2024_Dashboard.pbix
│
├── reports/
│   ├── figures/              # Grafici esportati dai notebook
│   └── summary.md            # Principali findings per ciascuna Q
│
├── requirements.txt
├── .gitignore
└── README.md
```

### File sorgente (`data/raw/`)

| File | Contenuto |
|------|-----------|
| *PDF 1* | Rapporto completo del Ministero della Salute — 2024 (con dati su farmaci, costi e ricoveri) |
| *PDF 2* | Sintesi ufficiale dei risultati dell'ultimo Report del Ministero della Salute |
| *Excel 1* | `Rapporto_SISM_appendice_2024.xlsx` — Tassi per 10.000 abitanti per fascia d'età e gruppo diagnostico |
| *Excel 2* | `Rapporto_SISM_tabelle_2024.xlsx` — 8 fogli: strutture, personale, prevalenza/incidenza, attività per setting |

---

## Fasi del Progetto

### Fase 1 — SQL
**Obiettivo:** estrazione, pulizia e preparazione dei dati per l'analisi.

Tecniche utilizzate: `JOIN` tra tabelle di prevalenza, strutture e continuità assistenziale · `GROUP BY` per aggregazioni regionali · Window functions (`RANK()`, `LAG()`) per ranking e variazioni anno su anno · `CASE WHEN` per segmentazione dell'utenza · Star Schema per la modellazione finale.

### Fase 2 — Python
**Obiettivo:** analisi statistica, esplorazione dei dati (EDA) e validazione delle ipotesi.

Tecniche utilizzate: EDA descrittiva con distribuzioni, heatmap e piramidi demografiche · Test statistici (ANOVA, Kruskal-Wallis) per differenze tra macro-aree · Regressione lineare sul trend 2015–2024 con analisi della discontinuità COVID-19 · Clustering k-means delle regioni per profilo assistenziale.

### Fase 3 — Power BI
**Obiettivo:** dashboard interattiva per la comunicazione dei risultati a stakeholder non tecnici.

Visualizzazioni principali: mappa coropleta delle regioni italiane · piramide demografica con slicer per diagnosi · line chart multi-indicatore con annotation sull'anno 2020 · funnel chart del percorso di cura (primo contatto → trattamento continuativo).

---

## 🔄 Pipeline del Progetto (In Corso)

- [x] **Fase 0:** Setup dell'ambiente, definizione della struttura e dei dati di partenza.
- [ ] **Fase 1 (SQL):** Importazione dei file Excel grezzi, gestione dei valori nulli/duplicati e modellazione del database (Star Schema).
- [ ] **Fase 2 (Python):** Analisi esplorativa dei dati, calcolo delle variazioni percentuali storiche e correlazioni statistiche.
- [ ] **Fase 3 (Power BI):** Sviluppo del modello dati, scrittura di misure DAX e design della dashboard interattiva.
- [ ] **Fase 4 (Insights):** Documentazione finale dei risultati principali in questo README.

---

## Autore

**Samantha Russo**  
Laurea in Psicologia · Corso professionalizzante in Data Analytics  
www.linkedin.com/in/samantha-russo-6756481b2(#) · https://github.com/SamanthaRusso01(#)

---

*Questo progetto è realizzato a scopo portfolio e utilizza dati pubblici del Ministero della Salute Italiano.*
