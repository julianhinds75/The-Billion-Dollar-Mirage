# 🎬 The Billion-Dollar Mirage  
**A Data Storytelling Project by Julian Hinds (2025)**  
*Exploring how global events, streaming, and franchise economics reshaped the modern film industry.*

---

## 🧭 Overview
Between 2000 and 2025 cinema reached record highs, collapsed during COVID-19, and re-emerged into a radically different world.  
This project blends **data analysis**, **visual storytelling**, and **business insight** to explain how billion-dollar blockbusters made Hollywood both stronger — and more fragile.

---

## 🎯 Objectives
- Quantify the rise and decline of global box office revenue.  
- Examine how streaming and pandemic behaviour changed audience habits.  
- Compare ticket price inflation vs real attendance.  
- Explore how independent films thrived under constraint.  
- Show how the gaming industry and attention economy reshaped entertainment.

---

## 🧩 Key Insights
1. **The COVID Cliff** – Global box office fell ≈ 80 % in 2020 and has not fully recovered.  
2. **Franchise Fragility** – MCU-era profits masked structural risk; post-2019 returns halved.  
3. **The Disney+ Effect** – Streaming turned studios into their own competitors.  
4. **Price ≠ Attendance** – Ticket prices more than doubled since 1996 while ticket sales fell ≈ 40 %.  
5. **Creativity in Constraint** – Micro-budget indies hit record ROI during lockdowns.  
6. **The Attention War** – AAA games (GTA VI, LoL) now out-perform films in 24-hour view counts and cultural pull.

---

## 🧮 Tech Stack & Structure
| Layer | Tools / Languages | Purpose |
|-------|-------------------|----------|
| **Data** | CSV → SQLite (`mirage.db`) | Easy, reproducible storage |
| **Analysis** | Python 3.11 • Pandas • Matplotlib • NumPy | Cleaning & visualisation |
| **Query** | SQL ( SQLite / DuckDB ) | Aggregations & joins |
| **Presentation** | Power BI / Markdown / PDF Report | Business-ready visuals |

### Repository Layout


---

## 📊 Datasets
| File | Description | Source |
|------|--------------|--------|
| `box_office_2000_2024.csv` | Worldwide film revenues | [Kaggle dataset](https://www.kaggle.com/datasets/parthdande/movies-box-office-collection-data-2000-2024) |
| `ticket_prices_uk.csv` / `ticket_prices_us.csv` | Historical ticket prices 1996-2024 | Comscore / The Numbers |
| `indie_roi_table.csv` | Lockdown-era indie film budgets & grosses | Compiled public sources |
| `trailer_views_24hr.csv` | Film vs Game trailer view counts | Official studio / press releases |
| `mirage.db` | SQLite DB built from all above CSV files | Generated locally |

Run the builder once:
```bash
python scripts/build_sqlite_db.py



# Create environment
conda env create -f environment.yml
conda activate mirage

# Launch analysis
jupyter notebook scripts/00_index.ipynb


-- Franchise share of global revenue
SELECT franchise, SUM(revenue_worldwide) AS total_rev, COUNT(*) AS films
FROM top100
GROUP BY franchise
ORDER BY total_rev DESC;


from scripts.plot_style import apply_style
with apply_style('dark'):
    ...



