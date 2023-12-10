# NBA Player Clustering
## Overview
This project performs cluster analysis on NBA player statistics to group players into functional categories based on their on-court statistics and style of play. The goal is to move beyond traditional position labels like "point guard" or "center" and instead look at how players actually perform using advanced metrics.

The analysis uses data from the 2020-2021 NBA season and considers statistics like points, rebounds, assists, blocks, field goal percentage, etc. Three clustering algorithms are tested - K-means, hierarchical, and model-based clustering. The optimal number of clusters is determined to be 3 based on multiple criteria.

The resulting 3 player clusters are characterized as:

**In-the-Paints**: High rebounds and blocks. Score efficiently inside but have poor outside shooting.

**Generals**: High points, assists, steals. Playmakers and scorers. Control tempo on offense.

**Versatiles**: Jack-of-all-trades. Don't stand out in any one stat but contribute across multiple categories.
Visualizations and statistical comparisons are used to profile each cluster. The analysis shows traditional position labels like "point guard" no longer adequately describe a player's role and style. The clusters provide an improved categorization of playing style in the modern NBA.

##  Code
The R code to perform the clustering analysis and generate visualizations is [here](https://github.com/omotuno/nba_positions_clustering/blob/main/NBA%20Positions.Rmd)). It does the following:

-- Loads and prepares the dataset

-- Removes unnecessary columns

-- Imputes missing 3-point percentage values

-- Resolves dual position labels using KNN

-- Clusters two datasets using K-means, hierarchical, and model-based algorithms

-- Determines optimal number of clusters

-- Compares cluster distributions across methods

-- Visualizes clusters through pairs plots, bar charts, etc.

-- Profiles and names the clusters based on their statistics

-- Analyzes Team USA and NBA championship teams

-- Results

## Key results and findings:

Traditional position labels like PG or C don't predict playing style/stats
3 clusters found to best categorize players: In-the-Paints, Generals, Versatiles
Each cluster has distinct statistical signatures related to scoring, playmaking, etc.
Playing style in NBA has evolved from the inside-focused 80s as the 3-point shot has become more emphasized
Team USA and NBA championship teams tend to be dominated by Versatile players
The analysis provides an improved, data-driven way to group NBA players based on their contributions rather than traditional notions of position.

## Next Steps
Potential extensions or future work:

-- Add more seasons of data for a timeseries analysis

-- Incorporate additional advanced metrics like PER, Win Shares, etc.

-- Look at team-level composition and performance for different mixes of clusters

-- Build interactive visualizations and a player recommendation tool
