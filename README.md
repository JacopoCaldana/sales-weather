# 🌦️ Sales & Weather Analysis Project

> Un progetto SQL per analizzare l'impatto delle condizioni climatiche sulle vendite, integrando dati di vendita e meteo in un’unica pipeline ottimizzata.

---

## 📌 Obiettivi del progetto

- Integrare dati eterogenei (vendite e condizioni meteo) in un’unica base dati relazionale.
- Ottimizzare la struttura delle tabelle SQL con vincoli e indici.
- Effettuare analisi avanzate sulle vendite condizionate da parametri climatici (temperatura, umidità, condizioni meteo).
- Sviluppare query SQL complesse (JOIN, nested, aggregazioni, condizioni multiple).

---

## 🛠️ Tecnologie utilizzate

- **SQL** (standard ANSI, testato su PostgreSQL e SQLite)
- **DBMS** (PostgreSQL, SQLite o altro compatibile)
- **Strumenti opzionali**: DBeaver, pgAdmin, SQLite Browser, Jupyter (per l’esecuzione integrata via Python-SQL)

---

## 📁 Struttura del progetto

''' 📦 progetto/
┣ 📂 sql/
┃ ┣ 📜 00_create_tables.sql         # Crea le tabelle raw di vendita e meteo
┃ ┣ 📜 01_create_view_weather.sql   # Crea la vista combinata dei dati meteo
┃ ┣ 📜 02_join_weather_sales.sql    # Join dati meteo e vendite
┃ ┣ 📜 03_clean_optimized_table.sql # Crea tabella pulita con indici e vincoli
┃ ┣ 📜 04_queries.sql               # Query di analisi avanzate
┃ ┗ 📜 README_queries.md            # Spiegazioni dettagliate query 11–19
┣ 📜 README.md                      # Questo file
┗ 📜 schema_diagram.png             # (opzionale) Diagramma ER delle tabelle '''


---

## 🧭 Step-by-Step – Come esplorare il progetto

### 🔹 1. **Creazione delle tabelle**
Esegui `00_create_tables.sql` per generare le tabelle:
- `orders_raw`
- `temperature`
- `humidity`
- `description`

### 🔹 2. **Creazione della vista meteo**
Esegui `01_create_view_weather.sql` per ottenere `combined_weather`, una vista che unisce temperatura, umidità e descrizione in base a data e ora.

### 🔹 3. **Join tra meteo e vendite**
Esegui `02_join_weather_sales.sql` per unire i dati delle vendite con quelli meteorologici.

### 🔹 4. **Pulizia e ottimizzazione**
Esegui `03_clean_optimized_table.sql` per creare `sales_weather_clean`, con:
- vincoli di chiave primaria/esterna
- indici sulle colonne di join
- dati standardizzati

### 🔹 5. **Analisi avanzate**
Esegui `04_queries.sql` per esplorare:
- pattern di vendita in condizioni meteo specifiche
- vendite medie per fascia di temperatura/umidità
- correlazioni tra meteo e volume di ordini
- nested queries, aggregazioni, subquery

> ✏️ Consulta `README_queries.md` per spiegazioni dettagliate sulle query dalla 11 alla 19.

---

## 📈 Risultati attesi

- Individuazione di pattern climatici che influenzano le vendite.
- Database efficiente e ben strutturato.
- Query avanzate eseguibili in tempi ottimali anche su dataset mediamente grandi.

---

## 📬 Contatti

Per domande o contributi:
- GitHub issues
- [Jacopo Caldana, Roberto Magno Mazzotta] – [Email]

---

## 🐣 Buona Pasqua e buon lavoro!  
Grazie per aver esplorato questo progetto 🌱
