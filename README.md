# NCAA Volleyball RAPM & Synergy Analysis

This repository contains a performance analytics project examining NCAA Division I Women's Volleyball using rally-level play-by-play data and Regularized Adjusted Plus-Minus (RAPM). The analysis focuses on player evaluation, positional tendencies, and lineup synergy within the Big Ten Conference.

## Overview

RAPM provides a framework for estimating player contributions to point-scoring independent of teammates, opponents, and game context. While commonly used in basketball, applying RAPM to volleyball introduces novel data and modeling challenges due to substitutions, rally scoring, rotations, and tracking of individual lineups.

The project leverages rally-by-rally data to:

- Reconstruct complete six-player lineups ("stints")
- Attribute point differential to lineup configurations
- Fit a ridge-regularized linear model to obtain RAPM estimates
- Compare results against official awards (e.g., All-Big Ten teams)
- Explore positional distributions and synergy metrics

## Key Components

### **Regularized Adjusted Plus-Minus (RAPM)**
- Built from thousands of rallies of play-by-play data
- Ridge-penalized linear model
- Produces player-level contribution estimates
- Validates volleyball-specific use cases of RAPM

### **Position-Based Distributions**
- Ridgeline plots visualize kill distributions by positional group
- Highlights role expectations for OH, OPP, MB, and Libero/DS

### **Lineup Synergy (Wisconsin Case Study)**
- Computes shared stint performance for player pairs
- Filters to well-sampled combinations
- Heatmap visualizes synergy using points per rally

### **Model Validation & Context**
- Compares top RAPM players against postseason awards
- Provides insight into how well RAPM aligns with coaching and media evaluations

## Data Sources

Play-by-play data sourced from:
- NCAA Division I Women's Volleyball (Big Ten Conference)

Season statistics:
- NCAA / Volleyball statistical reporting services
