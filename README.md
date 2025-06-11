# FIFA-Club-World-Cup-2025

This project is a data analysis and machine learning tool designed to evaluate and predict the performance of the football teams participating in the FIFA Club World Cup 2025. By leveraging predicted team performance data and integrating with generative artificial intelligence, the project offers in-depth analysis and creates fantasy lineups.

## Key Objectives and Functionality:##

1. **Team Performance Analysis:**
- ***Core Metrics:*** The project utilizes static data, including Opta Ratings and special predicted performance scores for three matchdays (`MD1`, `MD2`, `MD3`), as well as their total (`Sum`).
- ***Correlation Analysis:*** It identifies relationships between various metrics, such as the correlation between Opta Rating and the total `Sum` score, to determine key success factors.

2. **Predictive Modeling:**
- ***Team Classification:*** Using Logistic Regression, teams are classified as "strong" or "weak" based on the median value of the `Sum` metric. The model assesses which factors are most important in determining a team's strength.
- ***Win Probability:*** A function is implemented to calculate the probability of one team defeating another, considering not only overall strength but also performance consistency.

3. **Clustering and Segmentation:**
- ***Pattern Recognition:*** Using *K-means clustering*, teams are grouped based on their predicted results across the three matchdays (`MD1`, `MD2`, `MD3`). This allows for the identification of "balanced" teams (consistent results) and "explosive" teams (with significant peaks and troughs).
- ***Stability Analysis:*** The standard deviation (MD_std) of scores over the three matches is calculated to distinguish the most stable and unpredictable teams.

4. **Interactive Visualization:**
- The project actively uses the Plotly Express library to create interactive charts that help visualize the data effectively:
    - Predicted team form dynamics from match to match.
    - Distribution of total `Sum` scores across all teams.
    - 3D visualization of team clusters.
    - A heatmap of correlations.

5. **Integration with Generative AI (Gemini):**
- ***Fantasy Lineup Creation:*** Based on the analysis performed, a detailed prompt is generated for the Gemini model.
- ***Strategic Approaches:*** The AI is tasked with proposing three different starting lineups for a fantasy tournament, each with its own strategy: "The Powerhouses," "The Consistent Performers," and "The Dark Horses."

## Technology Stack: ##

- **Data Analysis:** Pandas, NumPy.
- **Machine Learning:** Scikit-learn (Logistic Regression, KMeans, StandardScaler).
- **Visualization:** Plotly Express, Matplotlib, Seaborn.
- **Generative AI:** Google Generative AI (Gemini).

This project serves as an excellent example of how modern data analysis and AI methods can be applied to gain a deep understanding of sports analytics and create engaging content for fans.
