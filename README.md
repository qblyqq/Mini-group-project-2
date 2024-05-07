# Mini-group-project-2
### HKUST (GZ) course project
This project uses Python with Dask to efficiently manipulate and analyze a comprehensive dataset on global trade. Our objectives include deriving descriptive statistics, identifying trade patterns through unsupervised learning, and predicting trade flows using machine learning techniques.

## Descriptive analysis
The project kicks off by identifying countries with the most and least trading partners, utilizing Dask's data frame capabilities for efficient computation. Further analysis extends into understanding overall trade volume and identifying sectors of highest value in the trade dataset.

### Top and Bottom Trading Countries
- Calculated the number of unique trading partners for each country.
- Identified the top 10 and bottom 10 countries based on the number of trading partners.

### Trade Volume and High-Value Sectors
- Merged product descriptions with trade data to categorize trade volumes.
- Highlighted sectors of economic significance, including petroleum, pharmaceuticals, metals, communications, and automobiles.

### Result illustrations
Using functions such as group by, trade data are explored
## <img width="233" alt="image" src="https://github.com/qblyqq/Mini-group-project-2/assets/158158854/c2974f41-4a65-4f5b-aacf-584174b8b2d0">
## <img width="463" alt="image" src="https://github.com/qblyqq/Mini-group-project-2/assets/158158854/46fabd40-010f-4834-9b71-e5497afd4d9f">
## <img width="294" alt="image" src="https://github.com/qblyqq/Mini-group-project-2/assets/158158854/e45a1409-602d-49d0-8059-28f46b587d3b">
## <img width="294" alt="image" src="https://github.com/qblyqq/Mini-group-project-2/assets/158158854/895372cb-6b25-40fe-9fc1-67dbf47a3f26">
## ![image](https://github.com/qblyqq/Mini-group-project-2/assets/158158854/4621b429-b7a9-4298-a48b-f09f656881f5)
## <img width="356" alt="image" src="https://github.com/qblyqq/Mini-group-project-2/assets/158158854/c2ca7837-7d9f-4c34-85f4-3936e3f252f4">

## Unsupervised Learning: Identifying Trade Patterns
Employing unsupervised learning techniques, we aim to uncover latent patterns in the global trade data. The approach involves normalizing data and applying K-means clustering to reveal clusters of countries based on their trading behaviors.

### Clustering Countries Based on Trade Patterns
- Applied K-means clustering to distinguish groups with similar export/import values and sectors.
- Utilized PCA for dimensionality reduction, aiding in visualization and analysis.
#### Result illustrations
<img width="554" alt="image" src="https://github.com/qblyqq/Mini-group-project-2/assets/94425924/308145d3-840c-4abd-b788-5a4b3ef6ab73">
<img width="686" alt="image" src="https://github.com/qblyqq/Mini-group-project-2/assets/94425924/90c8e093-8368-4076-884a-f2248f832c05">

## Machine Learning: Predicting Trade Flows
A machine learning model predicts export quantities based on several features including distance, GDP, and specific sectors. Feature engineering and hyperparameter tuning are conducted to enhance model performance.
### Model Building and Evaluation

- Split the dataset into training and testing sets.
- Utilized RandomForestRegressor for predictions.
- Evaluated the model using metrics such as MAE, MSE, and R^2 scores.

### Predictions for New Country-Sector Pairs
- Predicted export quantities for unseen country-sector pairs.
- Discussed the implications and limitations of using machine learning in trade flow predictions.
  
## Bonus Questions: Economic Implications of Distance on Trade
Exploring the impact of distance on exporting commodities, focusing on transportation costs and the nature of the goods. This section theorizes how distance influences trade patterns and proposes an analytical framework for further investigation.

### Economic Theory and Data Requirements

- Outlined the necessity of export data, distance metrics, and transportation cost information.
- Theorized the relationship between transportation costs, the nature of goods, and distance.

#### Details
- Economically, the impact of distance on exporting commodities is related to transportation costs and the nature of the goods being traded. 
- Transportation Costs: The farther a commodity needs to travel to reach its market, the higher the transportation costs. The heavier a commodity is, the higher the cost.
- Nature of Goods: Different commodities have different sensitivities to distance.
  - Perishable items like fruits and vegetables suffer more from long distances due to spoilage risks.
  - On the other hand, high-value goods like electronics might be less affected by distance because transportation costs form a smaller part of their overall value.
- Data Needed:
  - Export Data: Detailed information on what each country exports and to where.
  - Distance Data: Distances between exporting countries and major trading partners.
  - Transportation Costs Data: Information on shipping costs, including rates and modes of transport.

### Analytical Framework
- Presented a structured approach for analyzing the impact of distance on trade patterns.
- Suggested comparative studies, regression analysis, and detailed sector-specific case studies.
#### Details
- Compare Distances: Calculate average distances for each commodity sector to different export markets.
- Cost Analysis: Analyze how transportation costs vary across sectors and how they relate to distance. (Regression analysis)
- Case Studies: Look at specific examples within sectors to understand how distance impacts trade.
