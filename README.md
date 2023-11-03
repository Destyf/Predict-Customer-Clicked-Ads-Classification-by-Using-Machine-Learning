# Predict-Customer-Clicked-Ads-Classification-by-Using-Machine-Learning
Tools : Google Colab Visualization : Seaborn and Matplotlib Library Dataset : Rakamin Academy


A company in Indonesia wants to assess the effectiveness of an advertisement they have aired. 
This is crucial for the company to understand the extent of the advertisement's reach, thereby 
attracting customers to view it. By analyzing historical advertisement data and uncovering 
insights and patterns, this can assist the company in determining their marketing targets. The 
focus of this case is to create a machine learning classification model that can accurately identify 
the right target customers.


## Steps:

1. EDA
2. Data Cleaning & Preprocessing
   - Handling Missing Value :
       - Daily Time Spent on Site (13): Imputed with the median value.


       - Area Income (13): Imputed with the mean value.


       - Daily Internet Usage (11): Imputed with the median value.


       - Male (3): Imputed with the mode value.

   - Correcting Dtypes : Change Data Type of Feature Timestamp to Datetime
   - Feature Extraction : Extract data from the 'Timestamp' column into year, month, week, and day
   - Remove /Drop Column : Drop columns 'Unnamed: 0', 'Area Income', 'Male', 'city', 'province', 'category', 'Timestamp'.
   - Feature Encoding : Encode column ‘Clicked on Ad'
   - Normalization Data : Normalization data using MinMaxScaler
   - Split Data :
        - X (Feature): Daily Time Spent on Site, Age, Daily Internet Usage, Year, Month, Week, Day
  
      
        - Y (Target) : Clicked on Ad
3. Data Modeling :
   - LogisticRegression
        - Accuracy : 0.96

   
        - Precision : 1.00


        - Recall : 0.93


        - F1-Score : 0.96


        - AUC : 0.99
     

    - Coefficients for top features:
        - Daily Internet Usage 0.080685
      
      
        - Daily Time Spent on Site -0.078246
4. Business Recommendation :
    - Optimize Website Engagement: Encourage customers to spend more time on website by enhancing user experience, providing valuable content, and ensuring easy navigation.
    
    
    - Target Low Internet Usage Segments: Identify customer segments with lower internet usage, as they are more likely to click on ads. Consider tailoring specific ad campaigns for these segments.


    - Segmented Ad Strategies: Since Daily Internet Usage and Daily Time Spent on Site have nearly equal influence, consider segmenting ad strategies based on these factors. For customers with high internet usage and low time spent on the site, focus on attention-grabbing ads. For customers with low internet usage and high time spent on the site, invest in engaging content and interactive ad formats.
5. Business Simulation
