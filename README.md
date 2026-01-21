# Bellabeat User Activity Analysis  
Google Data Analytics Capstone Project

## 📍 Business Task
The objective of this analysis is to identify trends in smart device usage data and provide actionable insights that can help Bellabeat improve its marketing strategy and better engage its users.

## 📊 Data Sources
This analysis uses the **FitBit Fitness Tracker Data**, which contains personal fitness data collected from Fitbit users.

The main datasets used were:

- **dailyActivity**: daily physical activity data including total steps, active minutes, sedentary time, and calories burned.
- **sleepDay**: sleep-related data including total minutes asleep and time spent in bed.

These datasets are relevant to the business task because they allow the analysis of user activity and sleep behavior, supporting data-driven marketing and product decisions for Bellabeat.

### Data Preparation Notes
- Rows with zero activity values were reviewed and considered valid, as they may represent days when users did not wear the device.
- Some users did not have sleep records for every day, which is expected behavior and was retained.
- Date fields were standardized to ensure consistency across datasets.
- Sleep and activity datasets were linked using **User ID** and **Date**.

## 🛠 Tools Used
- SQL (data exploration and aggregation)
- Tableau (data visualization and dashboard creation)
- Excel (initial data inspection)

## 📈 Key Visualizations

### 1. Average Daily Steps per User

This visualization shows how users’ average daily steps vary over time, helping identify general activity patterns and consistency.

### 2. Steps vs Sedentary Minutes
A scatter plot analyzing the relationship between total daily steps and sedentary minutes.  
This visualization helps determine whether higher activity levels are associated with reduced sedentary behavior.

### 3. Steps vs Calories Burned
This scatter plot shows the relationship between daily steps and calories burned.  
Users with higher average daily steps tend to burn more calories, suggesting a positive relationship between physical activity and energy expenditure.

Initial visualizations showed inflated values due to total aggregation across users and days.  
Measures were corrected to **average daily values** to accurately reflect individual user behavior.

### 4. Sleep vs Activity
This visualization combines sleep and activity data to analyze the relationship between average daily steps and total minutes asleep.  
A trend line was added to highlight overall patterns.

## 🔍 Key Insights

- Users who take more daily steps generally burn more calories, confirming a strong link between physical activity and energy expenditure.
- Higher step counts are associated with lower sedentary minutes, indicating that more active users tend to spend less time inactive.
- The sleep vs activity analysis shows a **slight negative relationship** between daily steps and total minutes asleep.
  - More active users tend to sleep slightly fewer minutes on average.
  - This may indicate shorter but potentially more efficient sleep among active users.
- Aggregating data at the daily average level provides a more accurate representation of individual behavior compared to total sums.

## 💡 Recommendations for Bellabeat

- **Promote balanced activity goals**: Encourage users to increase daily steps while maintaining healthy rest and recovery habits.
- **Highlight efficiency over quantity**: Marketing messages can focus on quality sleep and efficient activity rather than simply longer sleep durations.
- **Personalized insights**: Bellabeat could provide users with personalized feedback combining activity, sedentary behavior, and sleep metrics.
- **Behavior-based engagement**: Target users with high sedentary time and low activity with motivational nudges and tailored content.

## 📊 Tableau Dashboard
A consolidated dashboard was created to summarize user activity, sedentary behavior, calories burned, and sleep patterns.

👉 <div class='tableauPlaceholder' id='viz1769019434749' style='position: relative'><noscript><a href='#'><img alt='Dashboard 1 ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Be&#47;BellabeatUserActivityAnalysis&#47;Dashboard1&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='BellabeatUserActivityAnalysis&#47;Dashboard1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Be&#47;BellabeatUserActivityAnalysis&#47;Dashboard1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='es-ES' /></object></div> 

---

## 📁 Repository Structure

data/ → Raw datasets

visuals/ → Dashboard and visualization images

README.md → Project documentation

---

## ✅ Conclusion
This analysis demonstrates how smart device data can be used to identify behavioral trends and support data-driven marketing strategies.  
The insights generated can help Bellabeat better understand its users and improve engagement through personalized, health-focused messaging.

