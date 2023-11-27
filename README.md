# Market Trend Analysis for Korean Products in the USA

1. Project Overview
2. Data Collection and Preprocessing
3. Data Visualization and Analysis
4. Model Building: LSTM Approach
5. Model Implementation and Deployment
6. Results and Business Impact
7. Conclusion
<br>

## **1. Project Overview**

### **Objective and Scope**
The primary objective of my project was to harness the power of data analytics to strategically identify and analyze potential markets for Korean-related goods and services within the United States. Targeting four major metropolitan states, my analysis aimed to uncover trends and preferences specific to Korean cuisine, tourism, culture, and especially cosmetics, which have been gaining global recognition.

The scope of my project extended beyond mere data analysis. It sought to provide actionable insights that could directly influence marketing strategies and decision-making. By focusing on metropolitan areas with diverse demographics and consumer behaviors, my research intended to pinpoint specific markets where Korean products and services could thrive.

### **Key Business Questions Answered:**
**Market Potential Assessment:** Which metropolitan state in the USA is the most promising for Korean goods and services, with an emphasis on the cosmetics industry?

**Trend Analysis:** What are the prevailing trends and consumer interests in Korean culture, cuisine, and tourism across these states?

**Correlation Insights:** How do the interests in various Korean-related categories correlate with each other, and what does this imply for integrated marketing strategies?
Through this project, I aimed not only to gather data but also to translate it into meaningful, market-specific strategies. The idea was to move beyond traditional analytics and offer a holistic view of the potential for Korean goods and services in the U.S. market, thereby enabling more informed and targeted marketing initiatives.
<br>
<br>

## **2. Data Collection and Preprocessing**

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

<br>
<br>

## **3. Data Visualization and Analysis**
Using Power BI, I conducted a detailed visualization of the data to unravel trends and interconnections. My dashboard was meticulously designed to provide comprehensive insights into the interest levels across different states for Korean-related goods and services.

**Key Elements of the Power BI Dashboard:**
- **Master Line Chart:** Displayed the absolute change in interest levels across all four categories (cuisine, tourism, culture, and cosmetics), segmented by state. It offered a dynamic view of how these interests evolved over time, providing a comparative analysis between states.
- **Significant Change Indicator:** Highlighted the most notable changes in interest levels, pinpointing the specific category and week when these shifts occurred. It served as a quick reference to understand sudden surges or declines in consumer interest.
- **Correlation Plot:** To explore the relationships between different categories, a correlation plot was included. This visual tool was instrumental in identifying how interests in Korean cosmetics correlated with other categories, such as cuisine, within each state.

**Key Insights Gained:**
- **Texas as a Focal Point:** The analysis revealed that Texas showed significant potential, particularly for Korean cosmetics and cuisine. This insight was pivotal in suggesting Texas as a prime target for focused marketing efforts.
- **Inter-Category Relationships:** The correlation plot unveiled a positive correlation between interests in Korean cosmetics and cuisine in Texas, suggesting a combined marketing approach could be effective.

Through these visualizations, I was able to transform raw data into actionable insights, laying the groundwork for data-driven marketing strategies. The Power BI dashboard not only enhanced my understanding of the current market dynamics but also provided a clear direction for future marketing initiatives targeting Korean goods and services in the United States.


<br>

## **4. Model Building: LSTM Approach**

The core of this project was the development of an LSTM (Long Short-Term Memory) model, designed to forecast future market trends for Korean-related goods and services. This model was meticulously constructed using Keras and TensorFlow, with a focus on capturing the nuanced temporal patterns in the data.

**Key Steps in Model Building:**

1. **Data Integration:**
   - Merged data from various sources to create a unified and comprehensive dataset for analysis.
   - Ensured data consistency and alignment to facilitate effective model training.

2. **LSTM Model Architecture:**
   - Developed a custom Sequential model incorporating LSTM and Dense layers, tailored for handling time-series data.
   - The LSTM layers were instrumental in capturing the sequential dependencies within the data.

3. **Training and Validation Process:**
   - Divided the dataset into training, validation, and test sets, following a systematic approach to prevent overfitting and underfitting.
   - Employed the training and validation sets to fine-tune the model, while the test set provided an unbiased evaluation of the model's performance.

4. **Hyperparameter Optimization:**
   - Conducted hyperparameter tuning to optimize the model's learning rate and the number of epochs, ensuring peak performance.
   - This step was critical in balancing the model's ability to learn from the data without losing generalization.

5. **Model Training:**
   - Trained the model over multiple epochs, monitoring key performance metrics like Mean Squared Error (MSE) and Mean Absolute Error (MAE).
   - Utilized a systematic approach to model training, ensuring each iteration brought improvements in predictive accuracy.

This phase was pivotal in translating raw data into actionable predictions. By harnessing the power of LSTM networks, I was able to build a model that not only understood the current market trends but could also predict future shifts with a significant degree of accuracy. This model served as a cornerstone for the project, enabling us to forecast market trends and make data-driven decisions. 

<br>

## **5. Model Implementation and Deployment**

In this final phase, I implemented and deployed the LSTM model to predict market trends using a Python script integrated with pytrends for dynamic data collection from Google Trends.

**Key Implementation Highlights:**

1. **Automated Data Retrieval:**
   - Implemented a Python script using pytrends to automate the collection of the latest Google Trends data.

2. **Data Preprocessing for LSTM:**
   - Structured the data specifically for LSTM input, using a windowed approach to align with time-series analysis.

3. **Model Deployment:**
   - Loaded the pre-trained LSTM model, leveraging Keras for time-series forecasting.

4. **Visualization of Predictions:**
   - Employed Matplotlib to visually represent both past trends and future predictions.

5. **GitHub Repository Management:**
   - Maintained a comprehensive GitHub repository documenting the project, including detailed Jupyter notebooks.

This phase showcased my ability to bring a data science project from concept to a practical application, emphasizing operational effectiveness and user-centric presentation. My work in this stage was focused on ensuring that the model's insights were both accurate and accessible, making it a valuable tool for understanding market trends in Korean-related goods and services.

<br>

## **6. Results and Business Impact**

The model's predictions provide insightful foresights into market trends, crucial for developing targeted marketing strategies in Texas for Korean products.

**Strategic Value:**
- Enabled data-driven decision-making for marketing Korean goods.
- Highlighted the significance of Texas as a potential market for expansion.
<br>

## **7. Conclusion and Future Work:**

The project successfully demonstrated the potential of data-driven approaches in market analysis. Future work includes expanding the analysis to other states and refining the model for even more accurate predictions.

**Future Directions:**
- Explore additional states for market potential.
- Enhance the model's accuracy and predictive capabilities.
