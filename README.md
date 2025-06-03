
# Travel & Hospitality(aviation)

### **Sky Analytics: Navigating the Complexities of Airline and Airport Operations**

### **Background:**

SkyNet Analysis Inc. is a leading consultancy firm specializing in aviation analytics. With the aviation industry's rapid expansion and the increasing complexity of global air travel, SkyNet plays a critical role in providing data-driven insights to airlines, airports, and regulatory bodies. The company has access to extensive datasets that cover a wide range of information, including flight schedules, delays, airline operations, and airport traffic details. These datasets offer a unique opportunity to explore and understand the multifaceted nature of the aviation industry, from operational efficiency and customer satisfaction to logistical challenges and environmental impact.

### Objective:

The primary objective of this case study, titled "Sky Analytics: Navigating the Complexities of Airline and Airport Operations," is to deeply analyze and interpret the extensive datasets encompassing flights, airlines, and airports - namely "flights.csv", "airlines.csv", and "airports.csv". The analysis aims to uncover critical insights into flight operations, delay patterns, airline efficiency, and airport traffic dynamics. By exploring these datasets, the study seeks to identify key factors influencing operational efficiency, understand the intricacies of flight scheduling and delays, and evaluate the performance metrics of airlines and airports. The ultimate goal is to provide strategic recommendations to enhance operational effectiveness, improve customer experiences in air travel, and contribute to the overall advancement of the aviation industry's standards and practices.

### **Data Source:**

1. **Flights Dataset**

[flights.csv](https://prod-files-secure.s3.us-west-2.amazonaws.com/d1e1bc70-9ede-4c69-84fd-42c5605803a0/ae2ac182-d6b6-4411-ad7e-3be1d7bc2a33/flights.csv)

This dataset contains detailed flight information, including timings, delays, and other flight-specific data.

- **YEAR, MONTH, DAY, DAY_OF_WEEK**: Date and day information for the flight.
- **AIRLINE**: Airline identifier.
- **FLIGHT_NUMBER**: Flight number.
- **TAIL_NUMBER**: Aircraft tail number.
- **ORIGIN_AIRPORT, DESTINATION_AIRPORT**: Airport codes for origin and destination.
- **SCHEDULED_DEPARTURE, DEPARTURE_TIME**: Scheduled and actual departure times.
- **DEPARTURE_DELAY**: Delay in departure (minutes).
- **TAXI_OUT**: The time duration between departure from the gate and wheels off.
- **WHEELS_OFF, WHEELS_ON**: Time when wheels were off/on the ground.
- **SCHEDULED_TIME**: Scheduled duration of the flight.
- **ELAPSED_TIME**: Actual time taken for the flight.
- **AIR_TIME**: Time in the air.
- **DISTANCE**: Distance covered by the flight.
- **TAXI_IN**: The time duration from wheels on to arrival at the gate.
- **SCHEDULED_ARRIVAL, ARRIVAL_TIME**: Scheduled and actual arrival times.
- **ARRIVAL_DELAY**: Delay in arrival (minutes).
- **DIVERTED, CANCELLED**: Indicators for diverted or cancelled flights.
- **CANCELLATION_REASON**: Reason for cancellation (if any).
- **AIR_SYSTEM_DELAY, SECURITY_DELAY, AIRLINE_DELAY, LATE_AIRCRAFT_DELAY, WEATHER_DELAY**: Different types of delays (minutes).

1. **Airlines Dataset**

[airlines.csv](https://prod-files-secure.s3.us-west-2.amazonaws.com/d1e1bc70-9ede-4c69-84fd-42c5605803a0/3632c550-cdbb-440f-a32b-90dbe4767865/airlines.csv)

This dataset provides information about various airlines.

- **IATA_CODE**: Unique airline code.
- **AIRLINE**: Full name of the airline.

1. **Airports Dataset**

[airports.csv](https://prod-files-secure.s3.us-west-2.amazonaws.com/d1e1bc70-9ede-4c69-84fd-42c5605803a0/1c354ebb-8057-4cf1-8d36-8a94c529bcd1/airports.csv)

This dataset contains information about various airports.

- **IATA_CODE**: Unique airport code.
- **AIRPORT**: Full name of the airport.
- **CITY**: City where the airport is located.
- **STATE**: State where the airport is located.
- **COUNTRY**: Country where the airport is located.
- **LATITUDE, LONGITUDE**: Geographic coordinates of the airport.

### **Part 1: Excel Data Analysis: Manipulation, Formulas and Functions**

1. **Missing Data Handling:** 
    - Identify and address missing data in the movies dataset. Are there any patterns in the missing data that can be noted?
2. **Flight Delays Analysis**:
    - Determine the average flight delay per airline. What are the top 3 airlines with the highest average delays?
3. **Airport Traffic Volume**:
    - Identify the top 5 busiest airports based on the number of incoming and outgoing flights.
4. **Flight Cancellation Insights**:
    - Analyze the flight cancellations: Which airline has the highest cancellation rate, and what are the most common reasons for cancellations?
5. **Seasonal Variations in Flight Operations**:
    - Examine if there are seasonal patterns in flight operations. Are certain months more prone to delays or cancellations?
6. **Correlation between Distance and Delays**:
    - Investigate if there's a correlation between the distance of the flight and the length of delays. Use scatter plots for visualization.
7. **Efficiency of Airlines**:
    - Calculate the on-time performance (percentage of flights that are not delayed) for each airline. Rank them based on this metric.
8. **Impact of Day of Week on Flight Operations**:
    - Assess how flight operations (delays, cancellations) vary by the day of the week.
9. **Analysis of Airport Connectivity**:
    - Which airports serve as the most significant hubs in terms of connectivity (most destinations served)?
10. **Flight Duration Accuracy**:
    - Compare the scheduled flight duration versus the actual flight duration. Which airlines have the most and least deviation?
11. **Airline Fleet Utilization**:
    - Based on the tail numbers, determine which airline has the highest number of flights per aircraft, indicating fleet utilization.
12. **Airport Geographical Analysis**:
    - Using latitude and longitude data, analyze the geographical distribution of airports. Which states or regions have the highest concentration of airports?
13. **Delayed Flights and Delay Types Analysis**:
    - For flights that are delayed, break down the delay types (airline, weather, security, etc.) and analyze their proportions.
14. **Long-Haul vs Short-Haul Operations**:
    - Compare the operational metrics (delays, cancellations) between long-haul and short-haul flights for different airlines.
15. **Pivot Analysis of Flights Data**:
    - Use pivot tables to summarize key operational metrics (like average delay, number of flights, cancellations) by airline and airport.
16. **Data Integration for Comprehensive Insights**:
    - Merge data from the "airlines.csv" and "flights.csv" to provide enhanced insights, such as correlating airline names with operational metrics. Analyze the merged data to determine the overall on-time performance of each airline, considering both arrival and departure delays.

16. **Airport Operations and Connectivity Assessment**:

- Combine the "flights.csv" dataset with the "airports.csv" based on airport codes. Use the merged dataset to identify the top 3 airports in terms of flight connectivity (number of unique destinations served) and analyze their average delay times (both departure and arrival).
1. **Flight Delay Impact Analysis**:
    - Calculate the cumulative impact of delays for each airline. Consider both the frequency of delays and the average delay time. How do these factors combine to affect overall airline performance?
2. **Optimal Flight Path Efficiency Assessment**:
    - Using the distance data from "flights.csv" and geographical coordinates from "airports.csv", calculate the efficiency of various flight paths. Determine if there are significant differences in the efficiency of flights (measured as a ratio of actual flight time to the shortest possible time based on distance) for different airlines or types of aircraft (identified by tail number).
3. **Airport Performance and Environmental Factors Correlation**:
    - Investigate if there's a correlation between airport performance (in terms of delays) and environmental factors like location (latitude and longitude from "airports.csv") and time of year (seasonal weather conditions). Are certain airports more prone to delays due to their geographical location and the associated weather patterns?
4. **Complex Delay Cause Analysis**:
    - Use nested functions to analyze the primary cause of delays for each airline. Determine if the predominant cause of delay (like airline delay, weather delay, security delay) varies by airline and time of day.
5. **Analysis of Flight Frequency and Peak Hours**: 
    - Analyze the flight frequencies to determine the peak operating hours for major airports. (Use a combination of Excel functions to categorize flights into different time slots (e.g., morning, afternoon, evening, night) and calculate the number of flights in each slot for the top 5 busiest airports.)

(Note: Show Vizualizations wherever possible in Part 1)

### **Part 2: Building an Excel Dashboard**

Create an interactive and dynamic Excel dashboard that provides a visual and analytical representation of key aspects of the aviation datasets. The dashboard should offer insights into flight operations, airline performance, and airport activity.

### **Key Components to Include in the Dashboard:**

1. **Flight Operations Overview**:
    - Incorporate a summary view showing total number of flights, average delays, and flight cancellations. Include filters to view data by specific airlines or airports.
2. **Airline Performance Analysis**:
    - Visualize performance metrics for each airline, such as average delay time, cancellation rates, and frequency of flights. Use charts like bar graphs or line charts for comparison.
3. **Airport Traffic Visualization**:
    - Display data on the busiest airports in terms of incoming and outgoing flights. Include interactive elements like a map for geographical representation and pie charts for traffic distribution.
4. **Delay Cause Breakdown**:
    - Provide a detailed analysis of the reasons for flight delays (weather, security, airline delays, etc.). Use a combination of pivot tables and stacked bar charts for this analysis.
5. **Time-based Flight Trends**:
    - Show how flight patterns and delay trends vary over different times of the day and across months. Implement a timeline or slider feature to allow users to explore temporal changes.
6. **User Interaction Features**:
    - Add slicers, dropdown menus, and timeline controls for users to interactively filter and explore the data across various dimensions like time periods, airlines, and airport codes.
7. **Dashboard Aesthetics and Usability**:
    - Ensure the dashboard is not only informative but also visually appealing and easy to navigate. Maintain a consistent color scheme and clear labels.
8. **Advanced Analysis (Optional)**:
    - If feasible, include a predictive analysis section where users can forecast future trends in airline performance or airport traffic based on historical data.
