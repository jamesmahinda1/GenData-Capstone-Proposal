# GenData-Capstone-Proposal
1. Project Overview

Project Title	S&P 500 Sector Performance Dashboard: Where Is the Market Actually Growing?
Tool	Microsoft Excel (Pivot Tables, Charts, Slicers, Conditional Formatting)
Dataset	S&P 500 Historical Stock Data — sourced from Kaggle (publicly available)
Dataset Size	Approximately 500 companies, 5 years of historical data (2019–2024)
Story Type	Trend and comparison analysis with an investment recommendation as the CTA

2. Problem Statement
Whenever people talk about the stock market, they usually treat the S&P 500 as one thing — "the market is up" or "the market crashed." But that framing hides something important: the 500 companies in the index are spread across 11 different sectors, and those sectors don't move together.

Some sectors thrived during COVID. Others got destroyed and never really recovered. Some look stable on the surface but are actually very volatile underneath. If you're trying to make any kind of informed investment or allocation decision, knowing "the market went up 10%" is not enough — you need to know which parts of the market drove that, and which parts are quietly dragging it down.

The question I want this dashboard to answer is:

"Which S&P 500 sectors have actually created value over the last 5 years — and which ones have been traps?"

3. How I Plan to Apply the Data Storytelling Framework
I'll be using the 6-step framework from the course to structure the whole project:

A — Audience
I'm targeting someone like a retail investor or a junior portfolio analyst — someone with decent financial literacy who doesn't have time to dig through raw data and just needs to know where to look. They care about returns, risk, and timing.

B — Context
Raw numbers don't mean much without something to compare them to. I'll add context through:
•	Historical comparisons — how each sector performed year over year
•	Benchmarking — each sector's returns vs. the overall S&P 500 average
•	Volatility — so you can see which sectors are high return but also high risk

C — Narrative Arc
I want the dashboard to tell a story with a clear beginning, middle and end:
•	Beginning: What did sector performance look like before COVID (2019 baseline)?
•	Middle: The 2020 crash — which sectors collapsed, which held up or even grew?
•	End: Post-recovery — who came out ahead, and what should someone do with that information?

D — Visuals
I plan to use a mix of charts so the data isn't just one wall of bars:
•	Line chart showing 5-year price trends per sector
•	Ranked bar chart of total returns, highest to lowest
•	Year-over-year clustered bar for side-by-side comparison
•	Heat map using conditional formatting for monthly returns

E — Emphasis
I'll make sure the most important insights are impossible to miss:
•	Top 3 sectors highlighted in green, bottom 3 in red
•	Key stat callouts per sector (e.g. "Technology: +185% over 5 years")
•	Chart annotations marking the COVID crash (March 2020) and the Fed rate hike period (2022)

F — Call to Action
I don't want the dashboard to just show what happened, I want it to point toward a decision. The final section will include a specific recommendation along the lines of:

"Based on 5-year risk-adjusted returns, a portfolio that overweights Technology and Healthcare while underweighting Energy and Utilities would have delivered around 40% higher returns at similar volatility levels. This suggests those two sectors are worth prioritising in any rebalancing decision."

4. Dashboard Layout Plan
The dashboard will have three main views, all connected through slicers so the user can filter by sector, year, or time horizon without touching any formulas:

View	What it shows	Excel features
Overview	KPI summary cards — best/worst sector, index average return, top mover YTD	MAXIFS, MINIFS, INDEX/MATCH, conditional formatting
Sector Trends	5-year price trend lines and a ranked bar chart of total returns per sector	Pivot charts, slicers by sector and year
Risk vs. Return	Scatter plot of average return vs. volatility, plus a monthly returns heat map	STDEV, pivot tables, colour scales

5. Data Source
•	S&P 500 Stocks dataset from Kaggle — daily historical OHLCV data for all S&P 500 companies
•	S&P 500 companies list — maps each ticker to its GICS sector classification
•	Both files are free, publicly available, and regularly updated

I'll use Power Query in Excel to clean and reshape the data before building the pivot tables and charts on top of it.

6. What I Expect to Deliver
By the end of the project, I want to hand in an Excel dashboard that:
•	Loads with an instant summary of the most important insights — no digging required
•	Lets the user filter by sector, year, and timeframe using slicers
•	Tells a clear story from pre-COVID baseline, through the crash, to who won the recovery
•	Ends with a concrete, data-backed recommendation the user can actually act on

The project will pull together everything covered in the General Data Analysis module — data cleaning, pivot tables, advanced formulas, visualisation, and the data storytelling principles from the guide.
