# Airbnb Listing EDA – New York 2024

---

## Project Overview

This project performs Exploratory Data Analysis (EDA) on New York City Airbnb listings to uncover trends and patterns in rental supply and pricing. We use Python libraries such as **pandas**, **NumPy**, **Matplotlib**, and **Seaborn** for cleaning, visualization, and analysis.

<img src="https://www.brandinginasia.com/wp-content/uploads/2017/04/sddefault-8.jpg" alt="Airbnb EDA">


---

## Objectives

The goals of this project are to:

1. Analyze room types, prices, and availability across neighborhoods and boroughs.
2. Understand host behavior and listing patterns.
3. Detect potential outliers in prices.
4. Provide actionable recommendations for guests and hosts based on insights.

---

## Dataset

The dataset contains **20,765** entries and **22** features, including:

- `id`: Unique identifier for each listing
- `name`: Title of the Airbnb listing
- `host_name`: Name of the host
- `neighborhood_group`: Borough where the listing is located
- `neighborhood`: Neighborhood of the listing
- `latitude`, `longitude`: Geolocation of listings
- `price`: Nightly rental price (USD)
- `room_type`: Type of accommodation (e.g., entire home/apt, private room)
- `number_of_reviews`: Total number of reviews
- `reviews_per_month`: Average monthly reviews
- `availability_365`: Number of days available in a year
- `last_review`: Date of the most recent review

> **Source:** Replace this line with your data source/link.

---

## Steps and Workflow

### 1) Data Cleaning

- Handled missing data in `price`, `neighborhood`, and `beds`.
- Fixed data types (e.g., converted `last_review` to `datetime`).
- Treated outliers by capping extremely high prices (e.g., values > $1,000) to reduce skew in visuals.

### 2) Exploratory Data Analysis (EDA)

1. **Room type distribution**
   - Visualized counts using bar plots.
   - Identified **Entire home/apt** as the most common room type.

2. **Neighborhood group (borough) insights**
   - Compared average prices across boroughs.
   - **Manhattan** shows the highest mean price.

3. **Availability trends**
   - Used correlation heatmaps among `price`, `availability_365`, `number_of_reviews`, and `beds`.

4. **Price distribution**
   - Plotted histograms and boxplots to inspect skewness and outliers.
   - Majority of listings fall in the **$50–$300** range.

5. **Host-level patterns**
   - Used boxplots/grouped views to analyze hosts with multiple listings.

6. **Review behavior**
   - Employed pair plots to explore relationships among `number_of_reviews`, `price`, and `availability_365`.

### 3) Data Visualization (Summary)

- **Pair plots:** Relationships among price, availability, and reviews.
- **Heatmaps:** Correlations among numerical features.
- **Histograms & Boxplots:** Price distribution and outliers.
- **Bar Charts:** Room types and borough distributions.

---

## Key Findings and Insights

### 1) Price Trends

- **Manhattan** has the most expensive listings, followed by **Brooklyn**.
- **Entire homes/apartments** cost significantly more than private or shared rooms.

### 2) Room Type Distribution

- Entire homes/apartments are most common; **private rooms** offer more budget-friendly options.

### 3) Outliers in Price

- A small number of listings priced above **$10,000** were detected; filtering or capping is recommended for robust analysis.

### 4) Availability Patterns

- Listings with **high availability** tend to have **lower prices** and often accumulate **more reviews**, possibly reflecting stronger demand at competitive prices.

### 5) Host Behavior

- Some hosts manage **multiple listings**, indicating a trend toward professional hosting.

---

## Recommendations

- **Guests:** Consider private rooms in Brooklyn or Queens for value; apply price filters around the $50–$300 range.
- **Hosts:** Benchmark against neighborhood medians; avoid extreme pricing without clear differentiators; monitor availability and adjust pricing dynamically.
- **Analysts:** Cap extreme outliers before modeling; stratify analysis by borough and room type.

---

## Future Work

- Train ML models (e.g., regularized regression, gradient boosting) to **predict price** from features like location, room type, and availability.
- Perform **sentiment analysis** on review text to quantify guest experience.
- Build an **interactive dashboard** (Plotly Dash/Streamlit/Tableau) for live exploration and monitoring.

## Contact
<u>
** LinkedIN: [LinkedIn](https://www.linkedin.com/in/ayush-kumar-maurya-a43914258/)<br>
** Twitter/X: [X](https://x.com/ayush_maur10241)
