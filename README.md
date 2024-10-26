# United States Broadband Availability - Availability Classification for October 2020
## Project Description
This project aims to analyze the availability category of broadband internet across U.S. counties as of October 2020. By exploring broadband distribution patterns and modeling classification based on availability, insights were gained into regional connectivity disparities and were able to identify areas with limited access. The project leverages machine learning techniques to classify broadband availability into high, medium, and low categories based on data from the Federal Communications Commission (FCC).

## Dataset Description
The dataset, sourced from the FCC, provides county-level broadband metrics, including the percentage of broadband availability and usage per county across the United States. Each record includes identifiers like county and state names, making it suitable for both regional analysis and aggregate modeling. Key fields include broadband availability, broadband usage, availability category, state average availability and usage, county identifiers.

## Summary of Findings
The analysis indicates that broadband availability vary significantly across counties and states. Areas with low broadband availability correlate with lower usage rates, highlighting access challenges. High broadband availability predominantly exists in urbanized regions, while rural counties often fall into medium or low availability categories. However, there are also instances where despite high broadband availability, the broadband usage is low. Which implies that there is a lack of proper use and infrastructure that lets users make full use of the available broadband. The Random Forest model proved to be the most accurate (100%) in classifying availability, underscoring its suitability for this classification task.

## Data Preprocessing
Cleaning Column Names: Removing extra leading whitespaces for consistent referencing.
Data Type Conversion: Converting availability and usage fields from string to numeric formats.
Handling Missing Values: Dropping rows with missing values in critical columns.
Feature Engineering: Creating availability categories (high, medium, low) based on predefined thresholds and calculating state-level average availability and usage for comparative insights.

## Exploratory Data Analysis
Histogram of Broadband Availability and Usage: Shows the distribution of availability and usage rates across counties.
Availability Category Counts: Displays the count of counties within each availability category (high, medium, low).
State-Level Averages: A bar and line plot compares average broadband availability and usage by state, highlighting regional differences.
Availability vs. Usage Scatter Plot: Demonstrates the correlation between broadband availability and usage across counties.
## Visualization
![Distribution of BROADBAND USAGE AND BROADBAND AVAILABILITY PER FCC](images/image1.png)
### "This chart illustrates the broadband usage and broadband availability between the different counties. The first plot shows a left-skewed distribution, which shows that there's a high broadband availability. The second plot shows that there's a right-skewed distribution which shows that there's a high count for low broadband usage."
![BROADBAND AVAILABILITY CATEGORY COUNTS](images/image2.png)
### "This chart categorizes the broadband availability category count. The graph shows that the highest count for the availability category is "HIGH", followed by "MEDIUM" and then "LOW"."
![State-level Averages of BROADBAND AVAILABILITY and BROADBAND USAGE](images/image3.png)
### "This chart shows the average broadband availability and usage in each state. States on the left show relatively low broadband availability and usage while states on the right show a much higher broadband availability and usage. States in between show a general but less consistent increase."
![BROADBAND AVAILABILITY PER FCC and BROADBAND USAGE SCATTER PLOT](images/image4.png)
### "This illustration shows the relationship between the broadband availability and usage. Each dot represents a data point, color-coded by availability: blue for low, purple for medium, and magenta for high. The graph shows a positive correlation, indicating that areas with higher broadband availability generally have higher broadband usage. However, inconsistency between usage and availability in some regions show that there may be other factors in play. Clustered points in the high availability categories show greater broadband availability coincides with increased usage but in some areas, adoption of broadband lags behind despite the presence of significant availability."


## Model Development
For classification, we explored several machine learning models:

Logistic Regression,
Random Forest,
Support Vector Machine (SVM),
K-Nearest Neighbors (KNN),

## Model Evaluation
The models were evaluated on their accuracy and classification metrics. The Random Forest model achieved perfect accuracy, making it the best classifier for broadband availability, followed closely by Logistic Regression with 99% accuracy. SVM and KNN models also performed well, achieving accuracies of 97% and 95%, respectively.

## Conclusion
This project highlights broadband accessibility trends across U.S. counties, identifying disparities in rural and urban regions. The Random Forest model’s accuracy validates its effectiveness in classifying broadband availability, aiding in identifying areas that may benefit from increased connectivity efforts. These insights provide a valuable resource for policymakers focusing on bridging the digital divide.
## Contributors
❗ NOTE: Your professor be the one to fill this section.
