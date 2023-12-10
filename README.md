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
The R code to perform the clustering analysis and generate visualizations is [here](https://github.com/omotuno/nba_positions_clustering/blob/main/NBA%20Positions.Rmd). It does the following:

-- Loads and prepares the dataset

-- Removes unnecessary columns

-- Imputes missing 3-point percentage values

<img width="688" alt="Screenshot 2023-12-10 at 4 13 46 PM" src="https://github.com/omotuno/nba_positions_clustering/assets/65866718/eec493ff-0891-41b8-8a83-6ee2af50be23">
<img width="677" alt="Screenshot 2023-12-10 at 4 14 19 PM" src="https://github.com/omotuno/nba_positions_clustering/assets/65866718/21e805fb-aaf0-404a-bcb1-dc7ea77070c7">



-- Resolves dual position labels using KNN



-- Determines optimal number of clusters

-- Compares cluster distributions across methods

<img width="685" alt="Screenshot 2023-12-10 at 4 15 16 PM" src="https://github.com/omotuno/nba_positions_clustering/assets/65866718/730eeb45-1110-4457-83df-fee7aec09ef9">

<img width="573" alt="Screenshot 2023-12-10 at 4 16 11 PM" src="https://github.com/omotuno/nba_positions_clustering/assets/65866718/743cc8d7-3488-4e99-890a-c8efe41b0804">

-- Clusters two datasets using K-means, hierarchical, and model-based algorithms
<img width="700" alt="Screenshot 2023-12-10 at 4 16 42 PM" src="https://github.com/omotuno/nba_positions_clustering/assets/65866718/a874fca4-4b50-4c4f-aeff-f7092e06d534">

<img width="703" alt="Screenshot 2023-12-10 at 4 16 58 PM" src="https://github.com/omotuno/nba_positions_clustering/assets/65866718/19a9716c-ecbf-487d-b838-84d964b05dc9">

<img width="629" alt="Screenshot 2023-12-10 at 4 17 16 PM" src="https://github.com/omotuno/nba_positions_clustering/assets/65866718/64cc01a8-1733-4298-83c2-7005c0410881">

<img width="682" alt="Screenshot 2023-12-10 at 4 17 34 PM" src="https://github.com/omotuno/nba_positions_clustering/assets/65866718/33bb03b3-2e0c-430f-946b-f08429b94cc0">

<img width="648" alt="Screenshot 2023-12-10 at 4 18 04 PM" src="https://github.com/omotuno/nba_positions_clustering/assets/65866718/7aec998e-4cd9-433f-8c22-1e6b3517f7f5">



-- Visualizes clusters through pairs plots, bar charts, etc.

<img width="612" alt="Screenshot 2023-12-10 at 4 18 18 PM" src="https://github.com/omotuno/nba_positions_clustering/assets/65866718/ccd60987-a003-46e5-adfc-39bc01a12ad9">

<img width="686" alt="Screenshot 2023-12-10 at 4 18 46 PM" src="https://github.com/omotuno/nba_positions_clustering/assets/65866718/998c76bb-97b0-45e3-b82a-4f06b5d0302d">

<img width="701" alt="Screenshot 2023-12-10 at 4 19 05 PM" src="https://github.com/omotuno/nba_positions_clustering/assets/65866718/b7bef51a-f74d-4a4c-b9f8-80e10a6046b8">

<img width="541" alt="Screenshot 2023-12-10 at 4 19 27 PM" src="https://github.com/omotuno/nba_positions_clustering/assets/65866718/82b97c0e-af18-478c-8aad-4fa6625a8cf0">

-- Profiles and names the clusters based on their statistics
<img width="692" alt="Screenshot 2023-12-10 at 4 19 48 PM" src="https://github.com/omotuno/nba_positions_clustering/assets/65866718/3a014c49-7c64-4650-85b8-f58c88ee4214">

<img width="695" alt="Screenshot 2023-12-10 at 4 20 06 PM" src="https://github.com/omotuno/nba_positions_clustering/assets/65866718/9f7bc94b-5278-4346-8196-3c545519dc4d">

<img width="688" alt="Screenshot 2023-12-10 at 4 21 56 PM" src="https://github.com/omotuno/nba_positions_clustering/assets/65866718/986bb730-87bb-479d-b662-48cc765fc03a">
<img width="700" alt="Screenshot 2023-12-10 at 4 22 13 PM" src="https://github.com/omotuno/nba_positions_clustering/assets/65866718/ade47675-accd-4cb0-800f-e6e6a2aa3013">

<img width="695" alt="Screenshot 2023-12-10 at 4 24 14 PM" src="https://github.com/omotuno/nba_positions_clustering/assets/65866718/93c5093e-4e1c-45bd-9d00-40a746d29f6f">

-- Analyzes Team USA and NBA championship teams

<img width="548" alt="Screenshot 2023-12-10 at 4 22 57 PM" src="https://github.com/omotuno/nba_positions_clustering/assets/65866718/1d82a228-3081-45af-b768-5d0fabde13b6">


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
