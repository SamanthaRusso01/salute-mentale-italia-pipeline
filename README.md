# 🧠 Analisi della Salute Mentale in Italia: Pipeline di Data Analysis (2015-2024)

Un progetto che ha L'obiettivo di ***tracciare l'evoluzione della salute mentale in Italia*** attraverso dati ufficiali, analizzando l'impatto demografico, le risposte dei servizi territoriali e i divari geografici, di genere e anagrafici.

---

## 🎯 Obiettivi del Progetto
Questo portfolio dimostra le competenze tecniche richieste per un ruolo di **Junior Data Analyst**, simulando una pipeline completa: dall'estrazione del dato grezzo fino allo storytelling visivo. Il progetto risponde a domande chiave come:
- Come sono cambiati i tassi di prevalenza dei disturbi mentali nell'ultimo decennio?
- Esiste un divario significativo di genere o di età nella diffusione della depressione?
- Quali regioni mostrano una maggiore pressione sui Servizi di Salute Mentale (CSM)?
- Come si correla il consumo di farmaci antidepressivi con l'ospedalizzazione?

---

## 🛠️ Tech Stack & Competenze Dimostrate
- **Data Architecture & Cleaning:** `SQL` per la pulizia, la normalizzazione delle tabelle ISTAT e la creazione di uno Schema a Stella.
- **Advanced Analytics:** `Python` (`pandas`, `matplotlib`, `seaborn`) per l'Analisi Esplorativa dei Dati (EDA) e lo studio dei trend storici.
- **Data Visualization & Storytelling:** `Power BI` (`DAX`, `Data Modeling`) per la creazione di una dashboard interattiva e parlante per gli stakeholder.
- **Version Control:** `Git` e `GitHub` per la gestione del codice e della documentazione.

---

## 📁 Struttura della Repository
La cartella di lavoro segue le pratiche standard di organizzazione dei progetti dati:
- 📁 `data/raw/` : Contiene i file sorgente originali non modificati:
  - 📄 *File PDF 1*: Analisi del 2021 sulla salute mentale in Italia (il documento di contesto da cui è nato l'idea del progetto).
  - 📄 *File PDF 2*: Ultimo Report completo del Ministero della Salute - 2024.
  - 📄 *File PDF 3*: Sintesi ufficiale dei risultati dell'ultimo Report del Ministero della Salute.
  - 📊 *File Excel 1*: Tabelle dati - Rapporto SISM_appendice_2024.
  - 📊 *File Excel 2*: Tabelle dati - Rapporto SISM_tabelle_2024. 
- 📁 `data/processed/` : Dataset puliti e pronti per l'analisi.
- 📁 `sql/` : Script `.sql` per la creazione del database, viste e query analitiche.
- 📁 `notebooks/` : Jupyter Notebook dedicati all'analisi statistica in Python.
- 📁 `powerbi/` : File `.pbix` contenente il modello dati e la dashboard finale.

---

## 📈 Pipeline del Progetto (In Corso)
- [x] **Fase 0:** Setup dell'ambiente, definizione della struttura e dei dati di partenza.
- [ ] **Fase 1 (SQL):** Importazione dei file Excel grezzi, gestione dei valori nulli/duplicati e modellazione del Database (Star Schema).
- [ ] **Fase 2 (Python):** Analisi esplorativa dei dati, calcolo delle variazioni percentuali storiche e correlazioni statistiche.
- [ ] **Fase 3 (Power BI):** Sviluppo del modello dati, scrittura di misure DAX e design della dashboard interattiva.
- [ ] **Fase 4 (Insights):** Documentazione finale dei risultati principali in questo README.

---
*Progetto sviluppato da <u>Samantha Russo</u>*
