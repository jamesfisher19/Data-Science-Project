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
- **Group by Industry**: Group data by industry and calculate the total layoffs and percentages for each.
- **Normalize**: Compare layoffs relative to the size of each sector to avoid misleading results from larger industries.
- **Chi-Square Test**: Perform a chi-square test to see if the distribution of layoffs across industries is significantly different.
- **Cross-Tabulation**: Use pivot tables to compare layoffs across industries during specific timeframes, such as recession periods.

### 3. What is the relationship between the amount of funds raised by a company and the likelihood or scale of layoffs?
- **Scatter Plot Data Preparation**: Extract relevant columns (e.g., `funds_raised`, `total_laid_off`) to observe trends.
- **Correlation Coefficient**: Calculate Pearson or Spearman correlation coefficients to assess the strength of the relationship.
- **Regression Analysis**:
  - Use linear regression to model the relationship between funds raised and total layoffs.
  - Check the regression coefficient to understand the magnitude of the relationship.
- **Categorical Comparison**: Divide companies into funding categories (e.g., low, medium, high funding) and compare average layoffs within each category.

### 4. Were there any periods of heightened layoffs that align with major economic or global events (e.g., pandemic waves, inflation spikes)?
- **Annotate Events**: Identify key dates for major events (e.g., COVID-19, inflationary periods) and align them with your timeline.
- **Compare Time Periods**: Split data into pre-event, during-event, and post-event periods to calculate total layoffs for each phase.
- **Statistical Tests**: Use t-tests or ANOVA to determine if layoffs during event periods are significantly different from other times.
- **Event Windows**: Analyze data in windows around key events (e.g., 3 months before and after) to assess impact duration.

### 5. Is there a correlation between the percentage of employees laid off and the stage of the company (e.g., startup vs. mature)?
- **Group by Stage**: Group data by stage (e.g., startup, mature) and calculate average `percentage_laid_off` for each group.
- **Box Plots or Summary Statistics**: Examine the distribution of layoffs within each stage.
- **ANOVA or t-tests**: Use statistical tests to check if the differences in layoff percentages between stages are significant.
- **Categorical Data Analysis**:
  - Create contingency tables comparing stage and percentage ranges.
  - Use chi-square tests to analyze patterns.

## Assumptions and Limitations

In this project, missing values in the `total_laid_off` column were replaced with `0`, based on the assumption that missing data likely indicates no layoffs were reported for those respective rows. This decision was made to simplify the analysis and ensure all rows contribute to trends and aggregates.

It is important to note that this assumption may not fully reflect reality, as missing data could also represent unreported layoffs or incomplete records. However, since this project is for learning purposes, this simplification was deemed acceptable to focus on exploring data manipulation and analysis techniques. 

This approach may introduce limitations, such as underestimating total layoffs or skewing results for specific questions, particularly those involving correlations or percentages. For professional or real-world applications, more rigorous imputation strategies or further investigation into missing data patterns would be necessary.