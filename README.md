# DSA-DATA-ANALYSIS-PROJECT-AMAZON-
This project was completed as part of a data analytics bootcamp, focused on deriving insights from Amazon product and review data. Using Excel and data visualization techniques, I explored patterns and trends to help improve product performance, marketing strategies, and customer satisfaction.

### Project Overview
The Amazon Product Analysis project focuses on understanding consumer preferences and market trends by analyzing a dataset containing 1,382 products across multiple categories, including Computers & Accessories, Electronics, and Home & Kitchen. The dataset is structured into multiple sheets, with key information on product pricing, discounts, ratings, and customer reviews. The primary objectives are:
- **Analyze Pricing and Discounts**: Evaluate the relationship between actual prices, discounted prices, and discount percentages to understand pricing strategies.
- **Assess Product Performance**: Investigate how ratings and rating counts correlate with product categories and price ranges.
- **Identify Category Trends**: Explore category-specific patterns, such as the prevalence of high discounts or high-rated products.
- **Customer Insights**: Examine customer reviews to identify sentiment and quality perceptions.

### Key Questions Answered:
1. What is the average discount percentage by product category?

2. How many products are listed under each category?

3. What is the total number of reviews per category?

4. Which products have the highest average ratings?

5. What is the average actual price vs discounted price by category?

6. Which products have the highest number of reviews?

7. How many products have a discount of 50% or more?

8. What is the distribution of product ratings?

9. What is the total potential revenue by category?

10. Product count per price bucket

11. How ratings relate to discount level

12. Products with fewer than 1,000 reviews

13. Categories with highest discounts

14. Top 5 products by ratings & review count


### Exploratory Data Analysis (EDA)
The EDA process involves cleaning, transforming, and visualizing the dataset to extract meaningful insights. Below is a summary of key findings and methodologies based on the provided dataset:

#### 1. Data Overview
- **Dataset Structure**: The dataset contains multiple sheets:
  - **Amazon Raw**: Raw data with 1,465 rows, including product details, customer reviews, and links (e.g., product IDs, names, categories, prices, ratings, and review content).
  - **Cleaned**: Processed data with calculated fields like Price Range, Potential Revenue, and Rating (>or<50%).
  - **Detail1**: Filtered data for Electronics|Mobiles category.
  - **Pivot**: Aggregated metrics like average discount percentages and rating counts by category.
  - **Visuals**: Summary of product counts per category.
- **Key Variables**:
  - **Product ID, Name, Category**: Identifiers and product classification.
  - **Discounted Price, Actual Price, Discount Percentage**: Pricing metrics.
  - **Rate, Rating Count**: Product quality and popularity indicators.
  - **Price Range**: Categorized as Cheap (<500), Expensive (500–2,000), or Very Expensive (>2,000).
  - **Potential Revenue**: Calculated as `Actual Price * Rating Count`.
- **Data Cleaning**:
  - Handled missing or truncated product names (e.g., "Wayona Nylon Br" in Cleaned sheet).
  - Addressed inconsistencies in category naming (e.g., "Computers Accessories" vs. "Computers&Accessories").
  - Removed duplicates and ensured consistent data types (e.g., converting prices to numeric).

#### 2. Key Insights
- **Category Distribution**:
  - The dataset includes 1,382 products across 18 categories, with **Home & Kitchen** (441 products), **Computers Accessories** (389 products), and **Electronics|Mobiles** (153 products) being the most represented.
  - Smaller categories like **Car Motorbike|Caracce** (1 product) and **Toys Games|Arts Craft** (1 product) indicate niche markets.
  
- **Pricing and Discounts**:
  - The average discount percentage varies significantly by category:
    - **Electronics|Wearablet**: 1.49 (highest, indicating aggressive discounting).
    - **Home & Kitchen**: 0.86.
    - **Electronics|Mobiles**: 0.88.
    - **Electronics|Poweracce**: 0.30 (lowest, suggesting stable pricing).
  - Products in the **Very Expensive** range (>2,000) dominate categories like **Electronics|Hometheat** (e.g., Samsung 80 Cm TV, ₹13,490) and **Electronics|Mobiles** (e.g., Samsung Galaxy, ₹37,990).
  - **Potential Revenue** is highest for high-rating-count products like **Amazonbasics Fl** (426,973 ratings, ₹298.9M potential revenue) and **Redmi 9A Sport** (313,833 ratings, ₹2.98B potential revenue).

- **Ratings and Popularity**:
  - Average rating counts are highest for **Amazonbasics Fl** (426,973), **Redmi 9A Sport** (313,833), and **Redmi 9 Activ** (313,836), indicating strong consumer engagement.
  - Products with discounts ≥50% tend to have higher rating counts, suggesting discounts drive popularity.
  - Ratings range from 2.9 (e.g., Ionix Tap Filter) to 4.6 (e.g., Sujata Dynamix), with most products averaging 4.0–4.5.

- **Customer Feedback**:
  - Reviews highlight product durability and charging speed for cables (e.g., Wayona Nylon Braided Cable: "Charging is really fast, good product").
  - Common complaints include quality issues (e.g., Bajaj Majesty RX10 Heater: "front part melted after 2 months") and slow performance (e.g., Havells Ventil Air Fan: "fan speed is very slow").
  - Sentiment analysis (to be implemented) could quantify positive vs. negative feedback.

#### 3. Visualizations
- **Discount Percentage by Category**: A bar chart showed **Electronics|Wearablet** and **Electronics|Headphone** with the highest average discounts, suggesting competitive pricing strategies.
- **Rating Count vs. Price Range**: A scatter plot indicated that **Cheap** products (<500) often have higher rating counts, likely due to affordability.
- **Correlation Analysis**: A heatmap revealed a moderate positive correlation (0.4–0.6) between discount percentage and rating count, suggesting discounts boost engagement.

#### 4. Tools Used

- Microsoft Excel

- Pivot Tables

- Calculated Fields

- Conditional Formatting

- Dashboards & Charts

