# Belly Button Biodiversity Dashboard

A cutting-edge web tool designed to explore the fascinating world of microbial diversity. Using advanced technologies like D3.js and Plotly.js, the dashboard transforms complex microbiome data into intuitive and interactive visualizations. Users can select individual samples to access detailed metadata and dynamic charts, providing a seamless and immersive experience for understanding the microscopic ecosystems within human belly buttons.

## Key Features
### Interactive Visualizations:
- **Bubble Chart:** Maps OTU (Operational Taxonomic Unit) relationships with clickable tooltips.
- **Bar Chart:** Displays the top 10 microbial populations for the selected sample.
- **Real-Time Updates:** The dashboard refreshes dynamically as users explore different samples.
- **Data-Driven Storytelling:** Combines powerful data visualization with engaging narratives to reveal the complexity of personal microbiomes.

## How It Works
### 1. Initialization
The `init()` function serves as the entry point for the dashboard. It:
- Fetches sample data from the dataset.
- Populates the dropdown menu with sample IDs.
- Displays metadata and visualizations for the first sample.

### 2. Metadata Panel
The `buildMetadata(sample)` function dynamically updates the metadata panel with detailed information about the selected sample ID. This includes:
- Demographic details.
- Microbial composition.
- Other relevant metadata.

### 3. Visualizations
The `buildCharts(sample)` function generates two key visualizations:
- **Bubble Chart:** Visualizes OTU relationships, with interactive tooltips for deeper insights.
- **Bar Chart:** Highlights the top 10 OTUs for the selected sample, making it easy to identify dominant microbial populations.

### 4. Interactive Experience
The `optionChanged(newSample)` event handler ensures a smooth and responsive user experience. Whenever a new sample is selected from the dropdown menu:
- The metadata panel updates instantly.
- The charts refresh to reflect the new sample’s data.

## Technologies Used
- **D3.js:** For dynamic and interactive data visualizations.
- **Plotly.js:** For creating rich and customizable charts.
- **JavaScript:** Powers the logic and interactivity of the dashboard.
- **HTML/CSS:** For structuring and styling the user interface.
