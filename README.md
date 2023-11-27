# Market Trend Analysis for Korean Products in the USA

## **Project Overview**
This project aims to analyze market trends for Korean-related goods and services in the United States, focusing on key metropolitan states. The objective is to identify potential markets for a targeted marketing campaign. The analysis revolves around various categories including cuisine, tourism, culture, and cosmetics, primarily utilizing Google Trends data.

**Key Business Question Answered:**
- Which metropolitan state in the USA shows the most promising market potential for Korean goods and services, particularly cosmetics?

## **Data Collection and Preprocessing**
Data was collected from Google Trends, focusing on four major states. The categories analyzed were cuisine, tourism, culture, and cosmetics. 

**Data Preprocessing Steps:**
- Averaging the search terms for each category, omitting zeros to address potential misspellings or alternative search terms.
- Consolidating data into a unified dataset for analysis.

## **Data Visualization and Analysis**
Using Power BI, we visualized the data to identify trends and patterns. 

**Key Insights:**
- Texas emerged as a promising market, especially for Korean cosmetics and cuisine.
- Positive correlation observed between interest in Korean cosmetics and cuisine in Texas.

## **Model Building: LSTM Approach**
An LSTM (Long Short-Term Memory) model was developed for forecasting future market trends. 

**Steps Involved:**
1. **Data Integration:** Unified multiple data sources for a comprehensive analysis.
2. **LSTM Model Development:** Custom Sequential model with LSTM and Dense layers, suitable for time-series forecasting.
3. **Training and Validation:** Split the data into training, validation, and test sets for robust model training.
4. **Hyperparameter Tuning:** Optimized the learning rate and number of epochs.

## **Model Implementation and Deployment**
Implemented a Python script using pytrends to fetch data automatically from Google Trends.

**Key Implementation Aspects:**
- **Automated Data Fetching:** Using pytrends for up-to-date Google Trends data.
- **Preprocessing and Windowing:** Prepared the data specifically for LSTM input.
- **Model Deployment:** Utilized the pre-trained LSTM model to make predictions.
- **Visualization of Predictions:** Displayed both historical data and future predictions graphically.

## **Results and Business Impact**
The model's predictions provide insightful foresights into market trends, crucial for developing targeted marketing strategies in Texas for Korean products.

**Strategic Value:**
- Enabled data-driven decision-making for marketing Korean goods.
- Highlighted the significance of Texas as a potential market for expansion.

## **Conclusion and Future Work**
The project successfully demonstrated the potential of data-driven approaches in market analysis. Future work includes expanding the analysis to other states and refining the model for even more accurate predictions.

**Future Directions:**
- Explore additional states for market potential.
- Enhance the model's accuracy and predictive capabilities.
