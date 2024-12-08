# Tech Layoffs Analysis (2020-2024)

## Description
This dataset documents tech layoffs reported from March 2020 to July 2024, offering valuable insights into workforce reductions during periods of economic downturn. Compiled using data from reputable sources such as Bloomberg, TechCrunch, and The New York Times, it provides a comprehensive view of the challenges faced by the tech industry.

This topic holds personal significance to me, as I have witnessed numerous people in my field endure repeated layoffs over the past few years (as of 2024). By analyzing and visualizing this data, I aim to better understand the realities of the industry and prepare for the challenges of navigating the modern workforce.

## Questions for Analysis

### 1. What trends can be observed in the number of layoffs over time (e.g., by month or year)?
- **Aggregate Data**: Group the dataset by time (month/year) to calculate total layoffs per time period.
- **Moving Averages**: Compute moving averages to smooth trends and identify patterns over time.
- **Statistical Analysis**: Use time series analysis techniques to identify peaks, troughs, and trends.

### 2. Are certain industries or sectors within tech more prone to layoffs during economic downturns?
- **Group by Industry**: Group data by industry and calculate the total number of layoffs for each sector. This highlights which industries experienced the highest layoffs over the analyzed period.
- **Visualize Industry Layoffs**: Create a bar plot to display total layoffs by industry, sorted in descending order. This provides a clear comparison across sectors and helps identify which industries were most affected.

### 3. Were there any periods of heightened layoffs that align with major economic or global events (e.g., pandemic waves, inflation spikes)?
- **Annotate Events**: Focused on two key events: the COVID-19 pandemic start (March 2020) and the inflation spike (November 2022).
- **Compare Time Periods**: Aggregated total layoffs for pre-event (3 months before), during-event (event month), and post-event (3 months after) periods for each event.
- **Visualize Layoffs**: Created a grouped bar chart to compare layoffs across the three periods for each event, highlighting changes during these critical times.

## Assumptions and Limitations

In this project, missing values in the `total_laid_off` column were replaced with `0`, based on the assumption that missing data likely indicates no layoffs were reported for those respective rows. This decision was made to simplify the analysis and ensure all rows contribute to trends and aggregates.

It is important to note that this assumption may not fully reflect reality, as missing data could also represent unreported layoffs or incomplete records. However, since this project is for learning purposes, this simplification was deemed acceptable to focus on exploring data manipulation and analysis techniques. 

This approach may introduce limitations, such as underestimating total layoffs or skewing results for specific questions, particularly those involving correlations or percentages. For professional or real-world applications, more rigorous imputation strategies or further investigation into missing data patterns would be necessary.