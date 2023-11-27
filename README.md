# Market Trend Analysis for Korean Products in the USA



## **Project Overview**

### **Objective and Scope**
The primary objective of this project was to harness the power of data analytics to strategically identify and analyze potential markets for Korean-related goods and services within the United States. Targeting four major metropolitan states, our analysis aimed to uncover trends and preferences specific to Korean cuisine, tourism, culture, and especially cosmetics, which have been gaining global recognition.

The scope of this project extended beyond mere data analysis. It sought to provide actionable insights that could directly influence marketing strategies and decision-making. By focusing on metropolitan areas with diverse demographics and consumer behaviors, our research intended to pinpoint specific markets where Korean products and services could thrive.

### **Key Business Questions Answered:**
- **Market Potential Assessment:** Which metropolitan state in the USA is the most promising for Korean goods and services, with an emphasis on the cosmetics industry?
- **Trend Analysis:** What are the prevailing trends and consumer interests in Korean culture, cuisine, and tourism across these states?
- **Correlation Insights:** How do the interests in various Korean-related categories correlate with each other, and what does this imply for integrated marketing strategies?

Through this project, we aimed not only to gather data but also to translate it into meaningful, market-specific strategies. The idea was to move beyond traditional analytics and offer a holistic view of the potential for Korean goods and services in the U.S. market, thereby enabling more informed and targeted marketing initiatives.


## **Data Collection and Preprocessing**

### **Data Collection**
Data was meticulously gathered from Google Trends, focusing on four major metropolitan states in the United States - known for their diverse demographics and potential market receptiveness. The primary objective was to analyze market trends for Korean-related products and services in these regions. The categories selected for this analysis were:

- **Cuisine:** kbbq, korean food, kimchi, korean restaurant, soju
- **Tourism:** korea flight, korea hotel, korea airbnb, korea vacation, korea tourism
- **Culture:** korean drama, kpop, korean movie, learn korean, kdrama
- **Cosmetics:** korean makeup, korean cosmetics, korean skincare, kpop makeup, korean beauty product

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
