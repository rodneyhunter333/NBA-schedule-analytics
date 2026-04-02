# NBA-schedule-analytics
Analysis of NBA schedule density, travel, rest, and win probability
# NBA Schedule Analytics: Travel, Rest, and Win Impact Modeling

## Overview
This project analyzes how NBA scheduling factors such as travel distance, rest days, and game density impact team performance. Using data from the 2019–2024 NBA seasons, I explored patterns in schedule difficulty and built a model to estimate how these factors influence game outcomes.

## Business Problem
NBA teams face varying levels of schedule difficulty due to travel, back-to-backs, and condensed game stretches. These factors can contribute to fatigue and impact performance.

This project answers:
- How does schedule density vary across teams and seasons?
- Which teams face the most demanding travel and rest conditions?
- Do scheduling factors meaningfully impact win probability?

## Data
- NBA game schedule data from the 2019–2024 seasons
- Derived features:
  - Rest days between games
  - Back-to-back indicators
  - Games in 6-night windows
  - Travel distance between games
  - Opponent win percentage

## Tools & Technologies
- R
- tidyverse
- dplyr
- lubridate
- ggplot2
- plotly
- geosphere
- Logistic Regression

## Data Cleaning & Preparation
- Converted game dates and calculated rest days between games
- Engineered schedule density features such as 4 games in 6 nights
- Calculated travel distance between consecutive games
- Removed inconsistencies and ensured games were ordered correctly
- Merged opponent performance metrics into the final dataset

## Exploratory Data Analysis
Key analyses included:
- Distribution of rest days across teams and seasons
- Frequency of back-to-backs and dense schedule stretches
- Team-level comparisons of schedule difficulty
- Travel burden analysis across seasons
- Visualizations showing schedule congestion patterns

## Modeling Approach
A logistic regression model was built to estimate the probability of winning a game based on:
- Home vs. away
- Opponent strength
- Rest days
- Back-to-back games
- Recent schedule density
- Travel distance

## Key Findings
- Teams experience meaningful variation in schedule density and travel burden
- Back-to-backs and condensed stretches are unevenly distributed across the league
- Opponent strength and home court had the strongest impact on win probability
- Schedule-related factors such as rest and travel showed smaller but measurable effects

## Business Impact
This analysis can support:
- Coaching decisions around player rest and rotations
- Front office planning for difficult schedule stretches
- Performance analysis tied to fatigue and travel
- Game preparation against stronger opponents under tighter rest conditions

## Files
- `schedule_project_complete.html` – full project output
- `README.md` – project summary and findings

## Next Steps
- Add player-level data such as minutes, injuries, and load management
- Test more advanced models
- Build an interactive dashboard version of the analysis
- Expand the work to explore playoff implications

## Author
Rodney Hunter
