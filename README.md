# belly-button-challenge


In this assignment, the JavaScript code utilizes the D3 and Plotly libraries to create an interactive dashboard for exploring the "Belly Button Biodiversity" dataset. This dataset catalogs the microbes present in human navels and provides insights into the diversity of microbial species, represented as Operational Taxonomic Units (OTUs). The dataset's analysis reveals that a few microbial species are commonly found in more than 70% of people, while the remaining species are relatively rare.

The interactive dashboard allows users to select different samples from a dropdown menu, and in response, it dynamically updates the displayed metadata and charts based on the selected sample. The dashboard presents key information about each sample, such as demographic data and microbial information, enabling users to explore the prevalence and abundance of different microbial species in human navels.

The main visualizations provided by the dashboard are:
1. Bar Chart: A horizontal bar chart showing the top ten OTUs present in the selected sample, ranked by their sample values (abundance). This chart allows users to quickly identify the most abundant microbial species in the navel sample.

2. Bubble Chart: A bubble chart that displays all OTUs in the selected sample. The size of each bubble represents the abundance of the corresponding OTU, and the color represents the OTU ID. This chart gives an overview of the diversity and distribution of microbial species in the sample.

3. Gauge Chart (not explicitly shown in the provided code): Presumably, this chart visualizes some information related to the selected sample, possibly a metric related to the overall biodiversity of the sample. However, the exact implementation of this chart is not shown in the provided code.

By building this interactive dashboard, users can gain valuable insights into the microbial diversity in human navels and observe the prevalence of specific microbial species across different samples. This tool may be helpful for researchers, students, and anyone interested in exploring and understanding the intricacies of human microbiota.

Explanation:

1. The code defines the URL from which to fetch the JSON data, and then uses D3 to read and log the data to the console.

2. The `init()` function is called when the page loads, and it performs the following tasks:
   a. It selects the dropdown menu element using D3.
   b. It fetches the JSON data from the provided URL and retrieves the sample names from the data.
   c. It populates the dropdown menu with the sample names as options.
   d. It selects the first sample from the list and then builds four initial plots (metadata, bar chart, bubble chart, and gauge chart) using the `buildMetadata`, `buildBarChart`, `buildBubbleChart`, and `buildGaugeChart` functions.

3. The `buildMetadata(sample)` function populates the metadata panel with information related to the selected sample. It filters the metadata based on the selected sample and appends key-value pairs to the metadata panel using D3.

4. The `buildBarChart(sample)` function builds a horizontal bar chart for the selected sample. It filters the sample data based on the selected sample, selects the top ten items to display, and then creates a Plotly trace for the bar chart with sample values on the x-axis and OTU (Operational Taxonomic Unit) IDs on the y-axis.

5. The `buildBubbleChart(sample)` function builds a bubble chart for the selected sample. It filters the sample data based on the selected sample and creates a Plotly trace for the bubble chart, with OTU IDs on the x-axis, sample values on the y-axis, and the marker size and color representing the sample values and OTU IDs.

6. The `optionChanged(value)` function is called when the user selects a different sample from the dropdown menu. It logs the newly selected value and then calls the four functions (`buildMetadata`, `buildBarChart`, `buildBubbleChart`, and `buildGaugeChart`) to update the dashboard with the data and charts for the new sample.

7. The `init()` function is called to initialize the dashboard when the page loads.

Overall, this code demonstrates how to use D3 and Plotly to create an interactive web visualization dashboard with dropdown functionality to select different samples and view corresponding metadata and charts.
