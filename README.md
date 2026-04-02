# Winning Space Race with Data Science

Project Overview: 
The primary goal of this project was to predict whether the Falcon 9 first stage would land successfully. Since SpaceX can reuse the first stage, they offer launches at approximately 62 million dollars, while other providers cost upward of 165 million dollars. Predicting successful landings allows for a more accurate determination of launch costs, providing a competitive edge for companies bidding against SpaceX.

Methodology:
- Data Collection: Information was gathered from the SpaceX REST API and via web scraping from the SpaceX Wikipedia page using BeautifulSoup.
- Data Wrangling: The dataset was cleaned by removing unnecessary data and null values. One-hot encoding was used to create a binary "Class" label (1 for success, 0 for failure).
- Exploratory Data Analysis (EDA): Insights were derived using SQL queries and various visualizations, such as scatter and bar charts.
- Interactive Analytics: Folium was used to generate interactive maps of launch sites, and a dashboard was developed with Plotly Dash to visualize success rates across different parameters.
- Predictive Analysis: Four classification models—Logistic Regression, SVM, Decision Tree, and KNN—were built and tuned using GridSearchCV to predict landing outcomes.

Key Insights:
- Temporal Trends: The success rate of stage 1 landings has generally improved over time, with the highest success rate observed in 2019.
- Orbit Performance: Orbits such as ES-L1, GEO, HEO, and SSO have achieved a 100% successful launch rate.
- Launch Site Geography: All launch sites are located near coastlines (Florida and California). KSC LC-39A handled the most successful landings but maintains a lower overall success rate compared to others.
- Booster Versions: The "FT" booster version category showed many successes, whereas "v1.1" recorded many failures.

Model Results:
- Accuracy: All models produced an identical accuracy rate of ~83.33% on the test data set.
- Confusion Matrix Analysis: The models correctly predicted all successful landings; however, they only correctly predicted half of the unsuccessful landings.
- Bias: The models tend to "over-predict" successful landings, resulting in false positives.

URL to course --> https://www.coursera.org/professional-certificates/ibm-data-science
This repository only cointains the last part of the course, the final capstone.
