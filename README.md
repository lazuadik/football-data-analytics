# Football Data Analytics

Match-level football analytics projects built with Python, from raw event data to insight.

| Project | Notebook | Article |
|---|---|---|
| Lamine Yamal vs Portugal, 2026 World Cup Round of 16 | [`Yamal-vs-Portugal-wc-2026.ipynb`](Yamal-vs-Portugal-wc-2026.ipynb) | [Medium](https://medium.com/@andhikarafilazuardi/lamine-yamal-vs-portugal-world-cup-2026-17a441fe292d) |

---

## Project: Lamine Yamal vs Portugal (World Cup 2026, Round of 16)

### Business question

Lamine Yamal entered the 2026 World Cup recovering from a hamstring injury (sustained 22 April 2026). Many expected the injury to limit his impact. **Did his performance against Portugal support that view?**

This was his first full 90 minutes of the tournament, which makes it the cleanest match to test the question.

### Approach

1. **Collect** match event data for Spain vs Portugal from [data source, e.g. provider name / URL].
2. **Clean and prepare** events for Yamal and his teammates with [pandas].
3. **Compute metrics**: passing accuracy, final-third and box passes, dribbles, shots, xG / xGOT, and touch distribution by pitch zone and flank.
4. **Visualize**: pass maps, shot map, dribble map and touch heatmaps with [matplotlib / mplsoccer].
5. **Compare** Yamal against his team (shot share, box deliveries) and against Baena on the opposite wing.

### Key findings

- **High involvement, not decisive.** Yamal completed 25 of 35 passes (71.4%) and 17 of 24 in the final third (70.8%), but had no goal or assist.
- **Contributed where Spain broke through.** He attempted 12 passes into the box and completed 5, accounting for 5 of Spain's 11 completed box passes (Spain attempted 39 in total).
- **Dribbling was mixed.** 3 successful dribbles from 8 attempts.
- **Shot volume without shot quality.** 3 shots (2 on target), about 20% of Spain's 15 shots, but only about 0.11 xG in total.
- **Role mirrored the opposite wing.** About 87% of his touches were on the right flank, with a final-third share similar to Baena's on the left.
- **Conclusion:** an active contributor in attacking play, not a match-winning display. Event data cannot measure sprinting or physical load, and one match is not enough to compare him with his pre-injury self.

> Full write-up with charts: [Medium article](https://medium.com/@andhikarafilazuardi/lamine-yamal-vs-portugal-world-cup-2026-17a441fe292d)

### Tech stack

- Python
- [pandas, NumPy]
- [matplotlib, mplsoccer]
- Jupyter Notebook

### Data

- **Source:** [provider name and link]
- **Coverage:** Spain vs Portugal, 2026 World Cup Round of 16 (event-level data)
- **Note:** [state whether raw data is included in this repo. If not, explain how to obtain it. Check the provider's terms before redistributing.]

### How to run

```bash
git clone https://github.com/lazuadik/football-data-analytics.git
cd football-data-analytics
pip install -r requirements.txt
jupyter notebook Yamal-vs-Portugal-wc-2026.ipynb
```

[If a data file or API key is required, describe it here. Never commit keys or tokens.]

### Limitations

- Single-match sample, so findings describe one game, not a trend.
- Event data does not capture off-ball movement, sprint speed or physical load.
- xG / xGOT values depend on the data provider's model.

---

## Other projects

- [End-to-End Football Analytics Pipeline](https://github.com/lazuadik/) (Premier League 2025/26): web scraping, Databricks ETL with PySpark (Bronze/Silver/Gold), star schema, Tableau dashboards. [Replace with the exact repo link.]

## Author

**Andhika Rafi Lazuardi**, Data Analyst
[LinkedIn](https://linkedin.com/in/andhikarafilazuardi) | [Medium](https://medium.com/@andhikarafilazuardi) | andhikarafilazuardi@gmail.com
