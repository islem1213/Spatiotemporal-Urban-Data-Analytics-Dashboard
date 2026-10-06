# Porto Motion

Interactive dashboard prototype for spatiotemporal mobility analysis in Porto. It demonstrates the product surface for ingesting bike-share, bus, and traffic data, surfacing congestion hotspots, corridor flows, and short-term demand forecasts.

## Motivation / research question

Porto’s open mobility feeds make it possible to observe individual services, but they do not readily answer a planning question that spans them: **where and when is mobility demand changing, and can the next-hour pressure on a zone or corridor be anticipated?** This project explores whether bike-share activity, bus movement, and traffic signals can be combined into a reliable, interpretable view of city movement. The aim is not only to display current conditions, but to test whether spatial hotspots, origin–destination flows, and short-horizon forecasts can surface actionable patterns for sustainable transport planning.

## Run

Open `index.html` in a browser. The UI is self-contained and uses simulated data so it runs without a backend or API key.

## Product scope

- Time and travel-mode controls update the live dashboard state.
- Heat/flow toggle changes the map treatment.
- Forecast panel visualises observed and modeled trip demand.
- Corridor and anomaly panels support operational triage.

The next production step is to wire the interface to source adapters, ETL, and a spatial store such as DuckDB Spatial or PostGIS.