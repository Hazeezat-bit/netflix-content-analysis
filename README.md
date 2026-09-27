# How Netflix Went Global — And What Happened Next

![Netflix Dashboard](netflix%20dashboard.png)
## The Question

By the mid-2010s, Netflix had a decision to make: keep growing as a primarily American movie service, or become something bigger. Did Netflix's massive catalog growth after 2016 come from doing more of the same — or from becoming a fundamentally different kind of platform?

I analyzed Netflix's full content catalog (8,807 titles, 2008–2021) to find out.

## What I Found

**Netflix didn't just grow. It transformed.**

In 2013, international content made up just 9% of everything Netflix added that year — the platform was overwhelmingly American. By 2018, that number had flipped: international titles made up nearly 70% of new additions. This wasn't gradual drift. It was a deliberate strategic pivot, and India led the charge — its share of new titles (among the top three producing countries) rose from 0% in 2013 to 35% by 2018, while the US's share fell to just over half.

**But the story has a twist.** After 2018, India's specific momentum cooled — its share dropped back down to around 14% by 2021, and the US climbed back up. If you only looked at the India numbers, you'd think the "global bet" reversed.

It didn't. Netflix's *overall* international content share stayed elevated — settling around 62–64% rather than falling back toward 2013 levels. In other words: **India sparked the pivot, but other countries carried it forward.** Netflix's globalization wasn't a single country's story — it became structural.

A few more pieces of the picture:

- **The pivot wasn't evenly spread across genres.** International growth concentrated heavily in "International Movies" and "Dramas" — this was a targeted expansion, not diversification for its own sake.
- **Content format shifted alongside geography.** International titles skew slightly more toward TV Shows than domestic titles do — the global pivot and Netflix's broader move into TV Shows appear connected, not coincidental.
- **Growth wasn't just about who — it was about how much.** Total content additions rocketed from a handful of titles per year before 2013 to over 2,000 in 2019 alone, with the international shift as the engine behind that acceleration.

## Why It Matters

This is a case study in how a platform outgrows its home market — not by accident, but by choice. Companies that hit ceiling growth in one market often face this exact decision: double down locally, or make a real bet on new geographies. Netflix's data shows what that bet looked like in practice — including the messy part, where the country that sparked the shift didn't stay the one carrying it. That nuance is the more useful lesson: **a strategic pivot can outlast the specific move that triggered it.**

If I were advising Netflix's content strategy team today, the follow-up question this raises is: which countries picked up the slack after India's contribution cooled — and is that growth as durable, or is Netflix now dependent on other markets in the same fragile way it once was dependent on India?

## Dataset

Source: Netflix Movies and TV Shows dataset (Kaggle)

The dataset contains 8,807 Netflix titles with information including:

- Title
- Content type (Movie or TV Show)
- Country
- Date added
- Release year
- Rating
- Duration
- Genres

## Tools Used

- Python (Pandas, NumPy, Matplotlib)
- Jupyter Notebook
- Tableau
- Git/GitHub

## Data Processing

The dataset was cleaned and prepared for analysis through the following steps:

- Converted `date_added` into datetime format and extracted year information
- Derived primary country from multi-country entries
- Filled missing categorical values with "Unknown"
- Removed 17 records with missing critical fields, representing less than 0.2% of the dataset
- Split multi-genre values from the `listed_in` column to enable genre-level analysis

## Dashboard

Interactive Tableau Dashboard — start on the **Summary** tab for the quick take, or explore the full dashboard for the details:

[https://public.tableau.com/app/profile/hazeezat.adebimpe.adebayo/viz/NetflixContentAnalysis_17905361175140/HowNetflixWentGlobal](https://public.tableau.com/app/profile/hazeezat.adebimpe.adebayo/viz/NetflixContentAnalysis_17905361175140/HowNetflixWentGlobal)

## Analysis Notebook

The complete Python analysis and data exploration can be found here:

[Netflix Analysis Notebook](Netflix.ipynb)

## Important Caveat — What This Data Can and Can't Tell Us

This analysis is based on Netflix's *catalog* — what titles were added and when. It reflects **what Netflix chose to stock, not what audiences chose to watch.**

That distinction matters here specifically. A company can pursue an international content strategy for reasons that have nothing to do with proven audience demand — tax incentives, licensing deals, local market entry commitments. So the finding this data actually supports is: **"Netflix pursued a deliberate, sustained international content strategy."** It does not tell us whether that strategy paid off in viewership or revenue — that would require data this dataset doesn't include.

Other limitations worth noting:

- Approximately 9% of titles have missing country information
- 2021 data represents a partial-year collection period
- The dataset represents a historical snapshot and does not reflect real-time Netflix catalog updates
