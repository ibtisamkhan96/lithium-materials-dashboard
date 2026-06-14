# Lithium, Materials Data Series #5

An interactive data dashboard and LinkedIn carousel on the metal that stores the energy: how little we mine, the two ways to get it, the China-dominated refining chain, and the wildest price ride of any major commodity.

Part of my Materials Data Series, where I take one material at a time and tell it as a materials engineer who works in data. Steel, aluminium, copper and rare earths came first. Nickel is next.

**Live dashboard:** _(deploy `index.html` to Netlify/GitHub Pages)_

---

## What's inside

| File | What it is |
|------|-----------|
| `index.html` | Interactive Chart.js dashboard, 5 tabs: Production & Geography, What 240 kt Looks Like, Brine vs Hard Rock, The Supply Chain, Boom Bust & Batteries |
| `fetch_data.py` | Reproducible Python pipeline that compiles the cited figures into `data/*.csv` |
| `data/*.csv` | Tidy datasets (production, extraction methods, China refining, reserves, trend, metals comparison, demand, price history, device content, scale) |
| `carousel/index.html` | 9-slide LinkedIn carousel (1080x1080) |
| `Lithium_Materials_Carousel.pdf` | Exported carousel, ready to upload |
| `linkedin-post.txt` | Post caption, with LinkedIn document title and GitHub slug at the top |

## Reproduce the data

```bash
python fetch_data.py      # writes data/*.csv
```

The dashboard embeds the same numbers in JS so it runs from `file://` with no server. `fetch_data.py` documents where each figure came from and keeps it reproducible.

## What the data shows

- The world mines only **240,000 tonnes** of lithium a year, a record, but we make more steel than that every hour.
- **Australia mines the most (~37%, hard rock), Chile pumps brine, and the lithium triangle (Bolivia, Argentina, Chile) holds 56% of reserves.**
- **Supply chain:** about **97% of Australian ore is refined in China**, which processes ~65% of all lithium. Owning the mine is not the same as controlling the metal.
- **Two extraction routes:** hard-rock spodumene (fast, ~16.7 kg CO2/kg) vs brine evaporation (cleaner at ~3.6 kg, but slow).
- **The most volatile major commodity:** lithium spiked ~10x into 2022, then crashed ~80% across 2023 to 2024. About 90% of demand is now batteries.

## Sources

USGS Mineral Commodity Summaries 2025 (production, reserves) · IEA Global EV Outlook (demand) · SMM and Benchmark Minerals (prices) · published life-cycle studies (extraction CO2).

Output in kt (thousand tonnes) of contained lithium; reserves in Mt lithium. Prices are approximate annual averages for battery-grade lithium carbonate. Figures rounded and attributed.

---

*Built by Ibtisam Ahmed Khan · June 2026 · [linkedin.com/in/ibtisam-ahmed-khan](https://linkedin.com/in/ibtisam-ahmed-khan)*
