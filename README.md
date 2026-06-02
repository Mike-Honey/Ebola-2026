# Ebola-2026

## DataViz project to analyse the 2026 outbreak of Ebola.

This analysis integrates the data on the DRC outbreak presented by [INRB-UMIE](https://github.com/INRB-UMIE/Ebola_DRC_2026?tab=readme-ov-file#readme). They are clearly putting a huge amount of work to rapidly gather and update information on this topic.

Part of their project gathers data from the daily situation reports and shares it as separate csv files per metric. My data pipeline attempts to integrate the detailed data (per Zones de santé / Health Zone) for flexible analysis.  So far I have integrated:

- insp_sitrep__cumulative_confirmed_cases__daily.csv 
- insp_sitrep__cumulative_suspected_cases__daily.csv

I am aggregating that detailed data to Province and national level. At present there are some discrepancies between those results and the project's own national totals, which they are working on resolving.
 

The tool I use is [Power BI](https://powerbi.microsoft.com/). This is an interactive data visualisation solution that allows interactive filtering and exploration of the data from any modern web browser.  

Note the images shown below are static screenshots - click on the links or the images to access the interactive dataviz, which will be refreshed regularly to integrate the latest available data.


### Metric Time Series by Geography

This page presents the sum of the selected Metrics by day as a time series (line chart) per geographic unit.  The user can select whether to view the national total, or break the series down by Province or DRC Health Zone.

Interactive "slicer" controls at the right of the page allow the user to restrict the date range, Metrics and Geographic Units shown.  

There's also a **Show top N** slicer to limit the number of series shown (by Metric value). This is intended to help review the data at DRC Health Zone level - there are many Health Zones with a handful of cases, which can lead to an overload in the number of series shown. 

A table at the bottom lists the detailed data. The table can be filtered by selecting series or points on the line chart.

[Link to interactive DataViz](https://app.powerbi.com/view?r=eyJrIjoiZTQ3MmNhZDYtMDFhMS00MDdmLWFlNjctYzUyMTNiNDZlMTdjIiwidCI6ImRjMWYwNGY1LWMxZTUtNDQyOS1hODEyLTU3OTNiZTQ1YmY5ZCIsImMiOjEwfQ%3D%3D&pageName=8f4bac1c6bb88bb2df35)

[![Click to view and interact with the report](https://github.com/Mike-Honey/Ebola-2026/raw/main/images/Ebola-2026-Metric-Time-Series-by-Geography.png)](https://app.powerbi.com/view?r=eyJrIjoiZTQ3MmNhZDYtMDFhMS00MDdmLWFlNjctYzUyMTNiNDZlMTdjIiwidCI6ImRjMWYwNGY1LWMxZTUtNDQyOS1hODEyLTU3OTNiZTQ1YmY5ZCIsImMiOjEwfQ%3D%3D&pageName=8f4bac1c6bb88bb2df35)


### Metric Time Series (Small Multiples)

This page presents each Metric as a "Small Multiple" - sub-charts which have a common Y-axis (Date). This can help compare the trends in the metrics.

Interactive "slicer" controls at the right of the page allow the user to restrict the date range and Geographic Units shown.  

[Link to interactive DataViz](https://app.powerbi.com/view?r=eyJrIjoiZTQ3MmNhZDYtMDFhMS00MDdmLWFlNjctYzUyMTNiNDZlMTdjIiwidCI6ImRjMWYwNGY1LWMxZTUtNDQyOS1hODEyLTU3OTNiZTQ1YmY5ZCIsImMiOjEwfQ%3D%3D&pageName=e803874f0ea76e3384c2)

[![Click to view and interact with the report](https://github.com/Mike-Honey/Ebola-2026/raw/main/images/Ebola-2026-Metric-Time-Series-Small-Multiples.png)](https://app.powerbi.com/view?r=eyJrIjoiZTQ3MmNhZDYtMDFhMS00MDdmLWFlNjctYzUyMTNiNDZlMTdjIiwidCI6ImRjMWYwNGY1LWMxZTUtNDQyOS1hODEyLTU3OTNiZTQ1YmY5ZCIsImMiOjEwfQ%3D%3D&pageName=e803874f0ea76e3384c2)


### Metric Time Series by Geography (Small Multiples)

This page presents each Geographic Unit (Province or DRC Health Zone) as a "Small Multiple" - sub-charts which have a common Y-axis (Date). This can help compare the trends in the Geographic Units.  The Geographic Units are shown sorted in descending order by their Metric value, so the most significant areas appear first.

Interactive "slicer" controls at the right of the page allow the user to restrict the date range, Metrics, Geographic Level and Geographic Units shown. There's also a **Show top N** slicer to limit the number of "Small Multiple" charts shown.

[Link to interactive DataViz](https://app.powerbi.com/view?r=eyJrIjoiZTQ3MmNhZDYtMDFhMS00MDdmLWFlNjctYzUyMTNiNDZlMTdjIiwidCI6ImRjMWYwNGY1LWMxZTUtNDQyOS1hODEyLTU3OTNiZTQ1YmY5ZCIsImMiOjEwfQ%3D%3D&pageName=58e8b6f4cd0bcc5d8000)

[![Click to view and interact with the report](https://github.com/Mike-Honey/Ebola-2026/raw/main/images/Ebola-2026-Metric-Time-Series-by-Geography-Small-Multiples.png)](https://app.powerbi.com/view?r=eyJrIjoiZTQ3MmNhZDYtMDFhMS00MDdmLWFlNjctYzUyMTNiNDZlMTdjIiwidCI6ImRjMWYwNGY1LWMxZTUtNDQyOS1hODEyLTU3OTNiZTQ1YmY5ZCIsImMiOjEwfQ%3D%3D&pageName=58e8b6f4cd0bcc5d8000)


### Page navigation

Once you have accessed a page in the interactive dataviz, you can access the other pages using the page navigation control at the bottom, which appears as: **< 1 of 3 >**

## Citations

- [INRB-UMIE Ebola DRC 2026 project](https://github.com/INRB-UMIE/Ebola_DRC_2026?tab=readme-ov-file#readme)
- **DRC health zones:** [Humanitarian Data Exchange](https://data.humdata.org/dataset/drc-health-data) (MoH zones de santé shapefile)
- **Epidemiological & operational data (INSP):** [Institut National de Santé Publique (INSP)](https://insp.cd/) SitRep MVE PDF series


## 🤝 Support

Contributions, issues, feature requests and sponsorship are all welcome!

Give a ⭐️ if you like this project!

[![Developed by a Human, not by AI. Click for more info](https://github.com/Mike-Honey/covid-19-au-vaccinations/raw/main/Developed-By-a-Human-Not-By-AI-Badge-white@2x.png)](https://notbyai.fyi)
