[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/1lXY_Wlg)

### Project Proposal: Weather-Triggered Food Campaigns Using Zomato Data

#### 1. Problem Statement

The objective of this project is to develop a system that uses weather data to trigger personalized food advertisements and restaurant suggestions for users. By leveraging the weather dataset from Zomato(See Doordash) - India's largest food delievery startup, we aim to enhance user experience by recommending food and restaurants that align with current weather conditions. This can help increase user engagement and satisfaction, and assist restaurants in managing demand more effectively.
Our idea is human craving for food is vastly dependent on the day-to-day weather, we'll be using the weather data collected from 60 cities with 1 minute refresh rate and calculating what kind of food items we should suggest our users, we also can help restaurants maintain load by forecasting the demand of the food.

#### 2. Project Scope

- **Data Collection**: Collect and integrate data from Zomato and weather APIs.
- **Data Processing**: Clean and preprocess the data, ensuring quality and consistency.
- **Data Storage**: Store the processed data in a suitable format for analysis.
- **Data Analysis**: Analyze the data to identify patterns and correlations between weather conditions and food preferences.
- **Implementation**: Develop a system to trigger ads based on real-time weather data.
- **Evaluation**: Assess the performance of the system and its impact on user engagement and restaurant demand.

#### 3. Datasets

- **Zomato Data**:
  - Format: JSON, CSV
  - Source: Zomato API and datasets
  - Content: Restaurant details, user reviews, menu items, location data, order history
  
- **Weather Data**:
  - Format: API (JSON/XML)
  - Source: weather Union API(Zomato), some other second weather API(Yet to be decided)
  - Content: Real-time weather conditions, forecasts, historical weather data

#### 4. Data Sources and Formats

- **Zomato API**: Provides JSON data for restaurant details, user reviews, and other relevant information.
- **Weather API**: Provides JSON/XML data for real-time weather conditions and forecasts.

The combined datasets will include at least 1 million rows, given the large volume of user reviews and historical weather data.

#### 5. Use Cases

- **Analytics Table in a Data Warehouse**: For in-depth analysis of user behavior patterns in relation to weather conditions.
- **Relational Database**: To store and manage data with complex relationships between users, restaurants, and weather conditions.
- **Dashboard**: For real-time monitoring and visualization of ad campaign performance and restaurant demand.

#### 6. Tech Stack

- **Data Collection and Integration**:
  - **Python**: For data extraction and API integration.
  - **Apache NiFi**: For automating and managing data flows.

- **Data Processing**:
  - **Pandas/Spark**: For data cleaning and transformation.
  - **Airflow**: For workflow orchestration.

- **Data Storage**:
  - **AWS S3**: For storing raw and processed data.
  - **Snowflake/Redshift**: For data warehousing and analytics.

- **Data Analysis**:
  - **SQL**: For querying and analyzing data.
  - **Jupyter Notebooks**: For exploratory data analysis.

- **Implementation**:
  - **Django/Flask**: For developing the backend system to trigger ads.
  - **JavaScript/React**: For frontend development of the dashboard.

- **Evaluation**:
  - **Tableau/Power BI**: For visualization and reporting.


#### 8. Detailed Eating Habits Table

| **Temperature Range** | **Rain Intensity** | **Total Rainfall** | **Humidity** | **Wind Speed & Direction** | **Eating Habits**                                                                                                                                                                |
|-----------------------|--------------------|--------------------|--------------|----------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Below 0°C (32°F)**  | Low to High        | Low to High        | Variable     | Variable                   | - High-fat, high-calorie foods to maintain body heat<br>- Hot meals and drinks (soups, stews, hot chocolate)<br>- Heavy, comforting dishes (casseroles, cheesy foods)<br>- Preserved foods (smoked meats, pickled vegetables) |
| **0°C to 10°C (32°F to 50°F)** | Low to Moderate | Low to Moderate | Moderate to High | Variable | - Warm, hearty meals (stews, roasted meats, baked dishes)<br>- Increased intake of root vegetables (potatoes, carrots, beets)<br>- Hot beverages (tea, coffee, hot cider)            |
| **10°C to 20°C (50°F to 68°F)** | Low to Moderate | Low to Moderate | Moderate to High | Variable | - Balanced diet with a mix of warm and cool foods<br>- Seasonal produce (apples, pears, leafy greens)<br>- Moderate intake of warm dishes and fresh salads                                  |
| **20°C to 30°C (68°F to 86°F)** | Low to Moderate | Low to Moderate | Moderate to High | Moderate | - Lighter meals with fresh ingredients (salads, sandwiches)<br>- Increased fluid intake (water, iced tea, fruit juices)<br>- Cold dishes (gazpacho, sushi, cold pasta salads)<br>- Hydrating foods (cucumbers, melons) |
| **Above 30°C (86°F)** | Low                | Low                | Low to Moderate | Moderate | - Very light meals, often cold or raw (fruit salads, smoothies, yogurt)<br>- High water content foods to stay hydrated (watermelon, citrus fruits)<br>- Cold desserts (ice cream, sorbets)<br>- Spicy foods to induce sweating (chili, curry) |

### Example Scenario

**Specific Weather Data:**
- Temperature: 23.4°C
- Rain Intensity: 0 mm/min
- Total Rainfall: 0 mm
- Humidity: 79%
- Wind Speed: 5.8 km/h

**Eating Habits:**
- **Light and Fresh Meals**: Considering the temperature (23.4°C), people might prefer lighter meals such as salads and sandwiches.
- **Increased Fluid Intake**: With moderate humidity (79%), hydration becomes essential, so consumption of water, iced tea, and fruit juices is likely.
- **Hydrating Foods**: Foods with high water content like cucumbers and melons will be popular.
- **Cold Dishes**: Cold pasta salads, gazpacho, and sushi can be appealing in this weather.

This fine-tuned table and example scenario provide a detailed analysis of how various weather conditions, including specific temperature and humidity, influence eating habits.

By incorporating the outlined eating habits table, we can tailor our food recommendations to better suit user preferences based on the weather, enhancing the effectiveness of the weather-triggered ad campaigns.
