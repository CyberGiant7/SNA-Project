# Social Network Analysis Project

## Overview

This project analyzes the global air transport network using various network analysis techniques. The goal is to identify key airports that play a pivotal role in global connectivity and understand the network's structure, robustness, and dynamics.

## Students

- [Leonardo Dessì](https://github.com/CyberGiant7)
- [Simone Rinaldi](https://github.com/simorina)
- [Filippo Brajucha]()
- [Gianmarco Gabrielli]()

## Project Structure

- `notebook.py`: Contains the main code for data preprocessing, network analysis, and visualization.
- `doc/doc.tex`: LaTeX document with detailed analysis and results.
- `data/`: Directory containing the OpenFlights data files (`airports.dat` and `routes.dat`).
- `images/`: Directory for saving generated plots and visualizations.

## Requirements

- Python 3.x
- `matplotlib`
- `networkx`
- `pandas`
- `powerlaw`
- `seaborn`
- `geopy`
- `geopandas`
- `folium`

Install the required packages using `pip`:

```sh
pip install -r requirements.txt
```

## Data Preprocessing

The project loads and processes airport and route data from OpenFlights CSV files. It cleans and filters the data, creates a weighted network of routes, symmetrizes the network, and builds an undirected graph with edges weighted by the number of routes and distances between airports.

## Network Analysis

The project performs various network analyses, including:

- **Centrality Metrics**: Degree, Degree Centrality, Betweenness Centrality, Eigenvector Centrality, Closeness Centrality, Clustering Coefficient, PageRank, Core Number.
- **Graph Metrics**: Density, Average Path Length, Diameter, Number of Connected Components, Assortativity, Number of Bridges.
- **Community Detection**: Using the Louvain method to identify regional clusters.
- **Robustness Simulation**: Analyzing the impact of removing the top 10 most connected airports on network connectivity, fragmentation, and compactness.

## Visualization

The project includes several visualizations:

- Network graph with nodes and edges.
- Interactive map visualization using `folium`.
- Bar plots for top airports by various metrics.
- Histograms for metric distributions in linear and log-log scales.
- Scatter plot for Clustering Coefficient vs Degree.
- Community clustering graph.
- Betweenness centrality changes after removing hubs.

## Results

The analysis highlights key insights into the global air transport network, including the identification of strategic airports, network robustness, and the overall structure and dynamics. The findings can improve route planning, air traffic management, and network resilience to disruptions.

## Conclusion

The project successfully identifies the most relevant and strategic airports in the global air transport network, demonstrating their importance in maintaining global connectivity. The analysis provides valuable insights for optimizing operations and ensuring the stability and reliability of air travel.

## License

This project is licensed under the MIT License.
