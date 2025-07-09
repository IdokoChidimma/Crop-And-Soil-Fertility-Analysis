# Crop-And-Soil-Fertility-Analysis
![Crop and Soil](https://github.com/user-attachments/assets/8dd51498-a2ab-48af-810b-312bd931bc4d)

## INTRODUCTION
  In today's agricultural practice, choosing the right crop for the right soil is critical for soil fertilty and crop production. As global food demand rises and soil degradation becomes more widespread and farmers face increasing pressure to optimize yield, reduce waste, resources and practice sustainability while navigating unpredictable climate conditions. This project addresses these challenges by presenting a crop recommendation system built on real world soil and crop data which aids farmers select the best crops to grow based on the specific properties of their soil. 

## OBJECTIVE
The primarly objective of this crop recommendation system is to provide accurate and relevant crop recommendation to farmers based on their soil characteristics and external environmental factors. This includes appropriate crops, advising on excessive fertilizer use, and providing irrigation methods to maximize productivity and enhance sustainability.
  
## 📊 WHY A CROP RECOMMENDATION SYSTEM?
   A Crop recommendation system helps in answering these question: "What is the appropriate crop to plant on specific soil type and condition"
 
  it does by analyzing:
 - Soil Nutrients: Nitrogen(N), Phosphorus(P), Potassium(K) also known as NPK
 - Soil pH
 - The Environmental/ Aboitic factors: Temperature, Moisture content and Humidity.

## 📂DATASET OVERVIEW
- **Data Source**:https://www.kaggle.com/datasets/shankarpriya2913/crop-and-soil-dataset

  - **Features include**:
  
  - Environmental conditions (Temparature, Humidity,	Moisture)
  - Soil Type
  - Crop Type
  - Nitrogen	Potassium	Phosphorous (NPK) levels
  - Fertilizer Name

## 🛠 Tools & Libraries
  The primary tools for developing this system is PYTHON, while other include;
  1. Pandas
  2. NumPy
  3. Seaborn, Matplotlib - Data Visulization
  4. Jupyter Notebook

## 🔬 Methodology

  This project began with the collection of a soil and crop dataset from Kaggle, which included variables such as crop type, soil nutrient levels (nitrogen, phosphorus, potassium), Fertilizer name, moisture, temperature, humidity, and soil types. The data was imported into jupyter notebook as Crop and Soil dataset.csv, then used data.shape to check for the number of rows and columns in the dataset which resulted to (8000, 9), checked for missing values, and standardizing formats. Exploratory Data Analysis (EDA) was conducted to understand the distribution of individual variables, to uncover patterns in how nutrient levels and environmental factors interact across different crops and soil types.
- Visualizations were created using Seaborn and Matplotlib to identify trends and correlations—such as how nitrogen levels increase with moisture, while phosphorus and potassium decrease, indicating leaching risks.

## 🔑 KEYS QUESTIONS AND INSIGHTS

### 1. What are the average Nitrogen, Phosphorus, and potassium levels required for different crops?
   
   📊 Insight:
   ![Average NPK Levels per Crop](https://github.com/user-attachments/assets/ddefa1a1-3a4c-4831-8871-fddadb825182)

   The average NPK (Nitrogen, Phosphorus, and Potassium) levels vary significantly across different crop types, highlighting the unique nutrient requirements of each. Among all crops analyzed, Millet, Barley, and Oil Seeds recorded the highest concentrations of soil nutrients, indicating that these crops either require or thrive in more nutrient rich conditions.
This variation is crucial for developing targeted fertilizer recommendations. For instance, high NPK demand crops like millet and barley may need nutrient enriched soils, while crops with lower NPK needs can be grown on less fertile soils to avoid over fertilization.

### 2. Which crops are most commonly represented in the dataset?
   
  📊 Insight:
  
  ![crop_distribution](https://github.com/user-attachments/assets/81b2e1d8-9537-4534-b8f6-d33847c77bd1)

 The bar chart illustrates the most frequently represented crops in the dataset, with Maize, Wheat, and Sugarcane emerging as the dominant types. Their high frequency suggests that these crops are likely of major economic and agricultural importance in the region where the data was collected. Identifying these key crops allows for focused soil treatment strategies, resource allocation, and targeted extension services. By prioritizing analysis and support for widely cultivated crops, policymakers and agronomists can make more impactful decisions.
 
### 3. What is the distribution of soil types across all crop samples?
   
   📊 Insight: 
   
   The dataset features a variety of soil types, but clayey and black soils appear most frequently, indicating they are widely used for cultivation in the region. These soils are known for their high nutrient-holding capacity and moisture retention, making them suitable for a range of crops. Understanding the prevalence of these soil types helps in designing location, specific for soil management practices and ensuring the right crops are matched to the right soil characteristics.

### 4. What is the typical pH range of the soils in the dataset, and are they suitable for common crpos?
   
   📊 Insight:
   
   ![Distribution of soil](https://github.com/user-attachments/assets/a373ae7b-c4aa-4121-985c-285aa63c9c81)
This histogram displays the distribution of soil pH values in the dataset. Most soil samples fall within a pH range of 5.5 to 7.0, which is generally favorable for crop growth. A pH range between 6.0 and 6.5 is often considered optimal, so it's encouraging that many samples lie within this window. However, a few samples fall into acidic (<5.5) or alkaline (>7.5) ranges, which may require soil treatment like limimg for optimal crop performance.
   
### 5. How does environmental factors (Temperature, Moisture, Humidity) influence soil nutrient levels (N, P, K)?

  📊 Insight:
  ![correlation_heatmap](https://github.com/user-attachments/assets/d824cf7b-3fac-43c6-b582-929ca0065088)
    Environmental Factors and Nutrient Correlation
    The analysis reveals that moisture levels negatively correlate with nitrogen but positively correlate with phosphorus and potassium. This suggests that while wetter soils may help retain phosphorus and potassium, they can also contribute to nitrogen leaching, reducing nitrogen availability for crops.
- In contrast, temperature and humidity show weak to moderate correlations with soil nutrient levels, indicating they have limited direct effects. However, their indirect impact such as influencing microbial activity, nutrient mineralization, and evaporation should not be overlooked, especially in region with low climate condition.

6. How do Nitrogen levels vary between different crop types?
   
#  📊 Insight:
![nitrogen_boxplot](https://github.com/user-attachments/assets/d1905abf-ea0e-412f-894f-28a5bdaa706c)
 This boxplot compares the distribution of nitrogen content across different crops. 
 - Crops like millet, maize and sugercane tend to require higher nitrogen levles as seen from their median values.
 -  others like barley, cotton show lower nitrogen dependency. Understanding nutrient requirements per crop helps in making informed fertilizer application decisions, improving yield and reducing waste.
   
7. How do Phosphorus levels vary between different crop types?

#  📊 Insight:
![Phosphorous_boxplot](https://github.com/user-attachments/assets/25a078dd-7250-44bf-b9b2-ddb295e57d42)

Phosphorus plays a important roles in root development, flowering, and seed development. The analysis shows that phosphorus levels are fairly consistent across most crop types, with only slight variations. 
- Crops like Barley, cotton and wheat appear to have slightly higher phosphorus, which indicate that they are phosphorus rich soils in the data.
- Others shows more moderate phosphorus levels, because they all fall within a similar range.
  
8. How do Potassium levels vary between different crop types?

#  📊 Insight:
![potassium_boxplot](https://github.com/user-attachments/assets/48159bbc-debc-4bd6-9a68-64ca773d4482)

Potassium is essential for water regulation, disease resistance, and crop quality.
- Potassium levels show more noticeable variation across crops compared to phosphorus.
- Oil seeds, Groundnuts, and Maize indicate higher potassium values, while Sugarcane and Millets show lower levels.
  

## ✅ RECOMMENDATION

# 👨‍🌾 For Farmers
- Crop rotation is a powerful and sustainable farming practice, To maintain soil fertility and improve nutrient balance, farmers should adopt strategic crop rotation based on the unique NPK demands of each crop. Alternate nitrogen-demanding crops (e.g., maize, wheat, sugarcane) with nitrogen-fixing legumes (e.g., beans, groundnuts). This naturally replenishes nitrogen in the soil, reducing the need for synthetic fertilizers.

- Adopt crop specific fertilization: Apply NPK fertilizers based on the crop’s average nutrient requirements rather than using general-purpose blends.

- Manage soil pH actively: For acidic soils, apply lime; for alkaline soils, consider sulfur amendments to bring pH into the optimal range (6.0–6.5).
  
- Monitor moisture levels: Maintain optimal soil moisture to support nitrogen availability, but beware of over-irrigation which may leach out phosphorus and potassium.

# 🧪 For Agronomists and Soil Scientists:
- Promote soil testing before planting to tailor fertilizer applications and improve yields.
  
- Develop decision support tools (dashboards, calculators) using insights from this analysis to guide smallholder farmers in optimizing nutrient use.
 nutrient behavior patterns.

# 🏛️ For Policy Makers and Extension Services:

- Support the access to soil testing kits and targeted fertilizers.
  
- Train extension workers to help farmers interpret soil pH, NPK readings, and make data-driven decisions.
  
 ## 🧾 Summary 
  This crop and soil fertility analysis reveals important interactions between soil nutrients, crop types, and environmental conditions. Most crops in the dataset such as maize, and sugarcane are grown in soils with a moderately acidic to neutral pH range (5.5–7.0), which promotes optimal nutrient availability and healthy crop development. Nitrogen levels show a strong dependence on soil moisture, whereas phosphorus and potassium levels tend to decline as moisture increases, likely due to nutrient leaching, While environmental factors like temperature and humidity have weak direct correlations with nutrient levels. This findings also support the use of crop rotation practices to maintain soil health and optimize nutrient usage across growing seasons.
