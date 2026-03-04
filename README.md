# Unsupervised Analysis of the U.S. Job Market

## Overview

-   **Course:** Advanced Modeling - Master's in Computational Social Science, UC3M

-   **Tools:** R, tidyverse, factoextra, cluster, ggplot2, plotly

-   **Methods:** Principal Component Analysis (PCA), K-Means Clustering, Hierarchical Clustering

## Project Description

This project analyzes 665 U.S. occupations to uncover hidden structure in the labor market using unsupervised learning. Data was merged from three public sources: BLS Employment Projections, Felten et al.'s AI Occupational Exposure (AIOE) index, and O\*NET work characteristics databases. They were merged using SOC occupation codes as the common identifier. The analysis examines whether occupations can be grouped into meaningful clusters based on labor market outlook, wages, and job characteristics, and what those clusters reveal about AI replacement risk.

## Key Features

-   Feature engineering and merging across 3 data sources via SOC codes

-   Exploratory data analysis including correlation analysis and distribution plots

-   PCA for dimensionality reduction and identifying main axes of occupational variation

-   K-means clustering with elbow method, silhouette scores, and gap statistic for k selection

-   Hierarchical clustering with Ward linkage, dendrogram, and phylogenic tree visualization

-   Cross-method comparison to validate cluster stability

## Files

-   `Unsupervised_USJobMarket.Rmd` - Main analysis script and R Markdown

-   `Unsupervised_USJobMarket.html` - Rendered report output — [view in browser here](https://htmlpreview.github.io/?https://github.com/oliviablantz/Unsupervised-Labor-AIRisk/blob/main/Midterm_Blantz.html)

-   `occupation.xlsx` - BLS Employment Projections data

-   `AIOE_DataAppendix.xlsx` - AI Occupational Exposure scores (Felten et al., 2021)

-   `Work_Activities.xlsx` - O\*NET Work Activities data

-   `Work_Context.xlsx` - O\*NET Work Context data

-   `midterm_data.csv` - Final cleaned and merged dataset

## Results

-   Four meaningful occupational clusters emerged consistently across both k-means and hierarchical methods.

-   The cluster with the highest AI exposure was dominated by cognitive, high-education occupations in management, legal, and computer science fields, reflecting a new trend that education and skill complexity do not necessarily provide job security in the age of AI automation.

-   Manual and trade occupations showed the lowest AI exposure, while a distinct cluster captured mixed, people-facing service roles.
