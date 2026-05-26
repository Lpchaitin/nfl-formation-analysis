# NFL Formation Analysis

## Overview
This project analyzes offensive vs defensive formation matchups across all NFL situations from 2016-2025. Using play-by-play data from nflverse and EPA as the primary evaluation metric, we identify which offensive formations and personnel packages perform best against specific defensive alignments across all downs, distances, and game situations.

## Key Questions
- Which offensive formations generate the most EPA against each defensive coverage type?
- Which personnel packages are most effective in the run game against different box counts?
- How do formation matchups change in the red zone vs open field?
- Which teams use formation advantages most effectively?

## Repo Structure
"""
nfl-formation-analysis/
├── data/
│   ├── raw/              # Raw play-by-play parquet files (not tracked)
│   └── processed/        # Cleaned dataset (not tracked)
├── notebooks/
│   ├── 01_data_exploration.ipynb
│   ├── 02_formation_overview.ipynb
│   ├── 03_offense_vs_defense.ipynb
│   ├── 04_run_game.ipynb
│   ├── 05_pass_game.ipynb
│   ├── 06_red_zone.ipynb
│   ├── 07_third_down.ipynb
│   └── 08_team_analysis.ipynb
├── outputs/
│   └── figures/
├── src/
├── requirements.txt
└── README.md
"""

## How to Run
1. Clone the repo
2. Install dependencies: `pip install -r requirements.txt`
3. Run notebooks in order: `01 → 08`
4. Data downloads automatically in notebook 01

## Data Source
Play-by-play data pulled via [nfl_data_py](https://github.com/nflverse/nfl_data_py) — credit to the nflverse contributors.