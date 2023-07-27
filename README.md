# belly-button-challenge


In this assignment, the JavaScript code utilizes the D3 and Plotly libraries to create an interactive dashboard for exploring the "Belly Button Biodiversity" dataset. This dataset catalogs the microbes present in human navels and provides insights into the diversity of microbial species, represented as Operational Taxonomic Units (OTUs). The dataset's analysis reveals that a few microbial species are commonly found in more than 70% of people, while the remaining species are relatively rare.

The interactive dashboard allows users to select different samples from a dropdown menu, and in response, it dynamically updates the displayed metadata and charts based on the selected sample. The dashboard presents key information about each sample, such as demographic data and microbial information, enabling users to explore the prevalence and abundance of different microbial species in human navels.

The main visualizations provided by the dashboard are:
1. Bar Chart: A horizontal bar chart showing the top ten OTUs present in the selected sample, ranked by their sample values (abundance). This chart allows users to quickly identify the most abundant microbial species in the navel sample.

2. Bubble Chart: A bubble chart that displays all OTUs in the selected sample. The size of each bubble represents the abundance of the corresponding OTU, and the color represents the OTU ID. This chart gives an overview of the diversity and distribution of microbial species in the sample.

3. Gauge Chart (not explicitly shown in the provided code): Presumably, this chart visualizes some information related to the selected sample, possibly a metric related to the overall biodiversity of the sample. However, the exact implementation of this chart is not shown in the provided code.

By building this interactive dashboard, users can gain valuable insights into the microbial diversity in human navels and observe the prevalence of specific microbial species across different samples. This tool may be helpful for researchers, students, and anyone interested in exploring and understanding the intricacies of human microbiota.


Instructions
Complete the following steps:

Use the D3 library to read in samples.json from the URL https://2u-data-curriculum-team.s3.amazonaws.com/dataviz-classroom/v1.1/14-Interactive-Web-Visualizations/02-Homework/samples.json.

Create a horizontal bar chart with a dropdown menu to display the top 10 OTUs found in that individual.

Use sample_values as the values for the bar chart.

Use otu_ids as the labels for the bar chart.

Use otu_labels as the hovertext for the chart.

bar Chart

Create a bubble chart that displays each sample.

Use otu_ids for the x values.

Use sample_values for the y values.

Use sample_values for the marker size.

Use otu_ids for the marker colors.

Use otu_labels for the text values.

Bubble Chart

Display the sample metadata, i.e., an individual's demographic information.

Display each key-value pair from the metadata JSON object somewhere on the page.

hw

Update all the plots when a new sample is selected. Additionally, you are welcome to create any layout that you would like for your dashboard. An example dashboard is shown as follows:

hw

Deploy your app to a free static page hosting service, such as GitHub Pages. Submit the links to your deployment and your GitHub repo. Ensure that your repository has regular commits and a thorough README.md file

Advanced Challenge Assignment (Optional with no extra points earning)
The following task is advanced and therefore optional.

Adapt the Gauge Chart from https://plot.ly/javascript/gauge-charts/Links to an external site. to plot the weekly washing frequency of the individual.

You will need to modify the example gauge code to account for values ranging from 0 through 9.

Update the chart whenever a new sample is selected.

Weekly Washing Frequency Gauge
