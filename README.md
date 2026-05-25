 # Soccer Match Analysis

  A comprehensive football match analysis notebook using StatsBomb event data, featuring the **2022 FIFA World Cup Final:
  Argentina vs France**.

  The notebook loads match event data via the `statsbombpy` package and generates visualizations and statistics including shot
  maps, pass networks, player heatmaps, defensive action maps, event timelines, and detailed player performance breakdowns.

  ## Features

  - **Match Overview** — lineups, formations, match info
  - **Basic Statistics** — shots, goals, passes, tackles, cards, etc.
  - **Shot Map** — pitch plot with all shots, sized by xG, colored by team
  - **Shot Details Table** — every shot with minute, player, xG, body part, situation
  - **Player Performance** — per-player stats: passes, shots, xG, tackles, interceptions, etc.
  - **Pass Network** — pass connection map showing team shape and key passing links
  - **Player Heatmaps** — hexbin touch maps for Messi and Mbappé
  - **Goal Timeline** — chronological listing of all goals with assist info
  - **xG Comparison** — bar chart comparing xG vs goals vs shots per team
  - **Passing Sonar** — top passers per team with accuracy percentages
  - **Defensive Actions Map** — tackles, interceptions, clearances, and blocks plotted on pitch
  - **Match Event Timeline** — goals, cards, and substitutions visualized chronologically
  - **Formation & Substitutions** — team setup and all changes made
  - **Duels & Possession** — duel win rates, ball recoveries, and possession estimates
  - **Summary Report** — auto-generated match summary with key insights

  ## Requirements

  - Python 3.8+
  - [statsbombpy](https://github.com/statsbomb/statsbombpy) — free StatsBomb event data access
  - mplsoccer — football pitch visualizations
  - matplotlib, seaborn, pandas, numpy, scipy

  Install dependencies:

  ```bash
  pip install statsbombpy mplsoccer matplotlib seaborn pandas numpy scipy

  Usage

  Open the notebook and run all cells:

  jupyter notebook soccer_analysis.ipynb

  Or with Jupyter Lab:

  jupyter lab soccer_analysis.ipynb

  The notebook fetches event data from StatsBomb's open-data repository on first run (internet connection required).

  Data Source

  All match data provided by StatsBomb (https://statsbomb.com/) via their free open-data API (statsbombpy).

  Match: Argentina 3-3 France (AET, 4-2 pens) — FIFA World Cup 2022 Final
  Match ID: 3869685
  Date: 2022-12-18
