# 🦅 Bird Stories of Newfoundland and Labrador

A data visualization project exploring bird sightings across Newfoundland and Labrador — uncovering seasonal migration patterns, geographic hotspots, and the role of protected areas in sheltering rare species.

Built as two complementary products: a **static infographic** for executive-ready storytelling and an **interactive dashboard** for hands-on exploration.

---

## 📊 The Infographic

A single-page visual narrative answering *when*, *where*, and *how protected* the birds of NL are.

![Bird Stories of NL Infographic](infographic_output.png)

### Key Findings
- **June** is the peak month, driven by summer breeding activity peaking at **9.8M sightings**
- The **Avalon Peninsula (St. John's)** alone accounts for **94% of all sightings** in the province
- **Ultra-rare species** are disproportionately concentrated inside protected areas — only **9%** of their sightings occur outside these zones
- Abundant birds appear inside protected areas at **75%** — 8.1x more than common birds

---

## 🖥️ The Interactive Dashboard

A Dash/Plotly web app that lets you explore the data yourself.

**Features:**
- 🗺️ **Animated migration map** — watch species move across the province month by month
- 🎛️ **Multi-filter sidebar** — filter by species, county, rarity tier, and protected area status
- 📈 **Dynamic KPI cards** — total observations, unique species, protected area %, and rarest species update instantly with every filter
- 📊 **Rarity distribution chart** — ranked 0–100, showing which birds are rarest in your selected area
- 🔢 **Linear / Log scale toggle** — switch scales on the protected area impact chart to compare tiers without common birds drowning out the rare ones

> **Example query:** Select *Bonavista* county + *Rare* tier + drag the slider to Month 9 → instantly see which rare birds pass through in September.

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| `pandas` | Data cleaning, ETL pipeline, rarity scoring |
| `numpy` | Percentile-rank calculations |
| `matplotlib` | Static infographic (multi-panel layout) |
| `plotly` | Interactive charts and geospatial map |
| `Dash` | Dashboard framework and callback logic |

---

## 📁 Project Structure

```
birds-of-nl/
├── Muhammed_Luckam_infographic_Project.ipynb   # Static infographic notebook
├── Muhammed_Luckman_dashboard_Project.ipynb    # Interactive dashboard notebook
├── birds.csv                                    # Source dataset (eBird NL records)
├── infographic_output.png                       # Final infographic export
└── README.md
```

---

## 🚀 How to Run

**Requirements**
```bash
pip install pandas numpy matplotlib plotly dash
```

**Infographic**
Open `Birds_of_NL_infographic_Project.ipynb` in Jupyter and run all cells. The infographic will render and save as `infographic_output.png`.

**Dashboard**
Open `Birds_of_NL_dashboard_Project.ipynb` in Jupyter, run all cells, then navigate to `http://127.0.0.1:8050` in your browser.

> Make sure `birds.csv` is in the same directory as both notebooks before running.

---

## 👥 Authors

**Muhammed Patel** — [LinkedIn](https://linkedin.com/in/muhammedpatel007) | [GitHub](https://github.com/muhammedp07)

*Memorial University of Newfoundland — Computer Science, 2026*
