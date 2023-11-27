# Market Trend Analysis for Korean Products in the USA

## **Project Overview**
This project aims to analyze market trends for Korean-related goods and services in the United States, focusing on key metropolitan states. The objective is to identify potential markets for a targeted marketing campaign. The analysis revolves around various categories including cuisine, tourism, culture, and cosmetics, primarily utilizing Google Trends data.

**Key Business Question Answered:**
- Which metropolitan state in the USA shows the most promising market potential for Korean goods and services, particularly cosmetics?
- 

## **Data Collection and Preprocessing**

### **Data Collection**
Data was meticulously gathered from Google Trends, focusing on four major metropolitan states in the United States - known for their diverse demographics and potential market receptiveness. The primary objective was to analyze market trends for Korean-related products and services in these regions. The categories selected for this analysis were:

- **Cuisine:** Exploring the interest in Korean cuisine, which includes traditional dishes and food items.
- **Tourism:** Assessing the popularity and demand for Korean-themed tourism and travel.
- **Culture:** Evaluating the influence and appeal of Korean culture, including entertainment and lifestyle aspects.
- **Cosmetics:** Investigating the market trends related to Korean cosmetic products, a rapidly growing segment globally.

### **Data Preprocessing Steps**
The data preprocessing phase was crucial in ensuring the accuracy and relevance of the analysis. The steps undertaken included:

1. **Keyword Selection and Search Term Analysis:**
   - For each category, multiple relevant keywords were chosen to capture a wide range of search interests related to Korean products and services.
   - These keywords were carefully selected to ensure they are representative of the categories in question.

2. **Averaging Search Terms:**
   - The average search interest for each category was calculated to get a more accurate and holistic view of the market trends.
   - Zeroes were omitted in this averaging process. This decision was made to avoid skewing the data due to potential misspellings, alternative search terms, or lack of data for certain terms, thereby ensuring more accurate and reliable results.

3. **Data Consolidation:**
   - The search data from Google Trends was consolidated into a unified dataset for each state.
   - This step involved aligning data across different timescales and ensuring consistency in the format for easier analysis.

4. **Data Cleaning and Formatting:**
   - The dataset underwent thorough cleaning to remove any inconsistencies, outliers, or irrelevant data points.
   - The data was formatted to fit the requirements of the subsequent analysis and modeling phases, ensuring smooth integration into the data visualization and machine learning pipelines.

Through these detailed and methodical preprocessing steps, the data was transformed into a format suitable for deep analysis, setting the foundation for insightful visualizations and predictive modeling.




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
