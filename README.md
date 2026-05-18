# Upstream-Aware Spatio-Temporal GNN for Crash Forecasting

This project develops a spatio-temporal graph neural network framework for forecasting crash risk on roadway segments. The model uses roadway network structure, upstream traffic patterns, and temporal crash-related features to predict future crash risk at the segment level.

## Overview

Crash risk is not only affected by conditions at a specific roadway segment, but also by traffic and safety conditions on nearby and upstream segments. This project represents the roadway system as a graph, where roadway segments are treated as nodes and their spatial connections are used to learn risk propagation patterns.

The goal is to forecast crash risk by combining:

- Spatial roadway network relationships
- Upstream segment influence
- Temporal traffic and safety patterns
- Graph neural network-based feature learning

## Motivation

Traditional crash prediction models often treat road segments independently or rely mainly on static roadway features. However, real traffic safety conditions are dynamic and spatially connected. Congestion, speed changes, weather effects, and upstream traffic conditions can influence downstream crash risk.

This project addresses that challenge by using a spatio-temporal GNN model that learns both network structure and time-dependent patterns.

## Methodology

The framework includes three main components:

### 1. Roadway Graph Construction

The roadway network is modeled as a graph:

- Nodes represent roadway segments
- Edges represent spatial connectivity between segments
- Directional connections are used to capture upstream and downstream relationships

This allows the model to learn how traffic and safety conditions propagate through the roadway network.

### 2. Upstream-Aware Spatial Learning

The model uses graph neural network layers to aggregate information from neighboring roadway segments. Upstream-aware aggregation gives special attention to upstream segments that may influence crash risk at the target segment.

This helps the model capture directional safety dependencies in roadway networks.

### 3. Temporal Crash Risk Modeling

Temporal features are used to capture how crash risk changes over time. The model learns patterns from historical sequences and predicts future crash risk for each roadway segment.

The temporal component can include features such as:

- Historical crash counts
- Traffic volume
- Speed
- Weather-related indicators
- Roadway conditions
- Time-of-day and day-of-week patterns

## Model Components

The framework may include:

- GraphSAGE-based spatial aggregation
- Directional upstream attention
- Adaptive gated fusion
- Temporal sequence modeling
- Segment-level crash risk prediction layer

## Evaluation Metrics

The model can be evaluated using classification or forecasting metrics depending on the task setup.

Common metrics include:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- MAE
- RMSE
- Segment-level prediction performance

## Key Features

- Spatio-temporal crash risk forecasting
- Roadway graph-based modeling
- Upstream-aware feature aggregation
- Directional traffic safety influence modeling
- Temporal sequence learning
- Segment-level crash risk prediction
- Useful for proactive road safety analysis

## Applications

This project can support:

- Roadway crash risk forecasting
- High-risk segment identification
- Traffic safety monitoring
- Proactive safety management
- Transportation agency decision support
- Data-driven roadway improvement planning

