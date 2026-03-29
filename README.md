# HW6
# Data Visualization: 
1. House Prices &
2. World Cup Networks

## Overview
This repository contains two distinct data visualization projects completed for HW6. The first part uses **R** to analyze and visualize historical housing and unemployment trends across US states.
The second part uses **Python** and **Cytoscape** to process and map a network of historical World Cup matchups (1930–2014).

## Part 1: US House Price Index Analysis (R)
This section analyzes the 'house_prices.rda' dataset to explore the relationship between housing prices and unemployment rates over time.

* **Tools Used:** R,-- 'dplyr', 'ggplot2','tidyr'--
* **Key Steps:**
  * Created small multiple line plots using 'facet_wrap' to show the 'house_price_index' trend for each state, specifically highlighting the years 1980, 2000, and 2020.
  * Reshaped the dataset using the 'gather' function to consolidate 'house_price_index' and 'unemploy_perc'into measure and value columns.
  * Generated a chart for each state to visually compare the housing index against unemployment percentages over time.
* **Outputs:** An R Markdown file and compiled HTML report containing the code, visualizations, and short analytical in markdown file.

## Part 2: World Cup Match Network Analysis (Python & Cytoscape)
This section processes the 'WorldCupMatches.csv' dataset to map how frequently national teams played each other.

* **Tools Used:** Python (Pandas), Cytoscape
* **Data Processing (Python):** * Addressed the "symmetric pair" problem by sorting team initials alphabetically, ensuring matchups were grouped correctly.
  * Grouped the data to calculate the total matches played between each pair  and the sum of all goals scored by the home teams.
  * Exported the cleaned data as csv(team_pairs.csv) file.(prepared this step to import in Cytoscape app.
* **Network Visualization (Cytoscape):**
  * **Nodes (Teams):** Ellipse shapes colored using a continuous gradient yellow to red based on the HomeGoalTeams.
  * **Edges (Connections):** Edge width and color are mapped continuously to the 'weight' column, highlighting the most frequent historical matchups with thicker, darker red lines.
  * **Layout:** yFiles Organic Layout.
* **Outputs:** The 'team_pairs.csv' dataset, the Python script/notebook, and a final image in .png of the final network graph.
