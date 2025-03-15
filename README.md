# ![CI logo](https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png)

## Genre Dominance Analyzer

The Genre Dominance Analyzer is a comprehensive data analysis tool designed to explore and visualize trends in video game genres from 1980 to 2023. Built with Python and Streamlit, this Data App provides an intuitive interface to uncover which genres have dominated the industry, how preferences have shifted over time, and which emerging genres show potential for growth. By delivering actionable insights, it aids game developers, publishers, and marketers in strategic planning for content development and marketing campaigns.

## Dataset Content

* Dataset: "Popular Video Games 1980 - 2023"
* Source: Kaggle - Popular Video Games 1980-2023
(https://www.kaggle.com/datasets/arnabchaki/popular-video-games-1980-2023)
* Description: This dataset contains detailed information on top-rated video games from 1980 to 2023, including titles, release dates, genres, platforms, average ratings, and playtime metrics (e.g., average and median playtime). It is publicly available, anonymized, and suitable for analyzing historical and current trends in the gaming industry without privacy concerns.

## Business Requirements

1. Market Insight: Identify which video game genres have consistently dominated the industry.
2. Track Genre Trends: Analyze how genre preferences have evolved across decades.
3. Highlight Emerging Genres: Identify niche or emerging genres with rising ratings or playtime that could signal future opportunities.
4. Support Strategic Decisions: Provide visual insights for game developers and marketers to plan content development and marketing strategies.

Key Questions:
1. Which genres have the highest ratings and popularity metrics?
2. How has the dominance of genres evolved from 1980 to 2023?
3. What correlations exist between genre, release frequency, and audience reception?

Value:

The tool supports game designers, publishers, and market analysts by informing strategic decisions regarding game development and promotional efforts.

## Hypotheses and Validation

* Hypothesis 1: "Action and Adventure genres have dominated the video game industry due to consistently high ratings and playtime across decades."
* Validation: Calculate average ratings and total playtime for each genre across the dataset, then visualize trends over time using a line plot and compare genre counts with a bar plot.
* Hypothesis 2: "Niche genres (e.g., Simulation, Strategy) show rising popularity in recent years based on increasing ratings and playtime."
* Validation: Filter data for the last decade (2013–2023), compute rating and playtime growth rates, and use a scatter plot to correlate these metrics with genre frequency.

## Project Plan
High-Level Steps:
1. Data Collection & Cleaning:

* Import the dataset.
* Clean and preprocess data (handle missing values, standardize genre names, etc.).

2. Exploratory Data Analysis (EDA):

* Conduct descriptive statistics and initial visualizations to understand data distribution.

3. Hypothesis Testing:

* Validate hypotheses using regression analysis, correlation metrics, and visualizations.

4. Dashboard Development:

* Create interactive visualizations (line plots, bar plots, scatter plots, heatmaps) using Plotly, Matplotlib, or Seaborn.
* Develop a user-friendly dashboard using Streamlit.

5. Deployment & Evaluation:
* Deploy the dashboard (e.g., on Heroku).
* Gather feedback from peers and iterate on improvements.

Data Management:
Collection: Data sourced from Kaggle.

Processing: Cleaned using Pandas in Jupyter Notebooks.

Storage: Organized into dedicated folders with version control via Git.

Interpretation: Insights are derived via statistical analysis and visualization.

## Data Analysis and Visualization
Techniques and Visualizations:

* Line Plot: Displaying genre rating trends over the years.
* Bar Plot: Showing top genres by rating count and release frequency.
* Scatter Plot: Visualizing the relationship between genre and release frequency.
* Heatmap: Presenting correlations between genres, ratings, and popularity metrics.

Rationale:
These visualizations map directly to our business requirements by highlighting dominant genres, trends over time, and underlying correlations.

Analysis Methods:

* Regression analysis for predictive insights.
* Clustering techniques to group similar genres.
* Correlation analysis to uncover interdependencies.

## Analysis Techniques Used
* Methods:
* Descriptive Statistics (mean, median, standard deviation of ratings and playtime using NumPy).
* Grouping and Aggregation (Pandas groupby for genre and decade summaries).
* Trend Analysis (time-series analysis of ratings by release year).
* Correlation Analysis (Seaborn heatmap for genre-platform interactions).

Limitations: Limited to historical data; lacks real-time player feedback.
* Alternatives: Could incorporate web-scraped review data, but avoided due to complexity and scope.
* Structure: Techniques applied sequentially—cleaning, summarizing, then visualizing—to ensure logical flow.
* Justification: Structured to mirror real-world EDA workflows, starting with data understanding and ending with insights.
* Data Limitations: Missing playtime for some games; filled with median values to avoid bias. No alternative datasets were needed.

## Generative AI Use
* Ideation: Used AI (e.g., Grok) to brainstorm project ideas and refine business questions.
* Design Thinking: AI suggested mapping visualizations to requirements, enhancing UX focus.
* Code Optimization: AI provided snippets for efficient Pandas filtering and Plotly styling, documented in Jupyter comments.

## Ethical Considerations
* Data Privacy: Dataset is anonymized and publicly available, posing no privacy risks.
* Bias: Older games may have fewer ratings due to less digital tracking; mitigated by focusing on relative trends.
* Fairness: Ensured genre categorization reflects original data, avoiding subjective reclassification.
* Legal/Social Issues: No legal concerns (public dataset); socially, insights avoid stereotyping genres or platforms.

## Dashboard Design

Pages and Widgets:

* Home Page: Overview of the project with key insights.
* Trend Analysis: Interactive line plots for genre trends over time.
* Detailed Analysis: Multiple tabs featuring bar plots, scatter plots, and heatmaps.
* Filters: Options to filter by year, genre, and platform.
* Narrative Section: Textual summaries explaining visual insights for both technical and non-technical audiences.
* Communication:
The dashboard uses clear labels, tooltips, and legends to explain the data insights. Interactive elements help users dive deeper into the analysis.

## Unfixed Bugs and Limitations
* Rendering Issues: Some visualizations may render slowly on lower-end devices.
* Data Gaps: Limited data for certain niche genres may affect analysis accuracy.
* Known Bugs: Minor issues in interactive filtering are documented and planned for resolution in future updates.
* Mitigation: Detailed documentation and planned roadmap for bug fixes.

## Development Roadmap
Challenges Faced:

* Data cleaning complexities due to inconsistent genre labels.
* Learning curve with advanced visualization libraries.

Strategies and Future Plans:

* Continue learning advanced data visualization techniques.
* Integrate real-time data updates for the dashboard.
* Explore additional machine learning models to enhance predictive capabilities.

## Credits and Acknowledgements
Content Sources:

* Dataset provided by Popular Video Games 1980-2023 on Kaggle.
* Visual design inspiration from various industry case studies.
* Technical guidance and code snippets inspired by online tutorials (e.g., YouTube, Kaggle kernels).

Acknowledgements:
Special thanks to mentors, peers, and the data science community for feedback and support throughout this project.