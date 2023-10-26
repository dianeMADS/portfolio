# A. SQL and NoSQL Databases
(under construction)

# B. Examples of Dashboards
1. Traffic Monitoring and Forecasting
2. MatPlotlib
3. Altair
4. Seaborn
5. Power BI

# C. Examples of Predictive Modelling nad Causal Inference
### C.1 Leveraging Machine Learning for Network Traffic Forecasting

[pdf]()

[notebook]()

Traditional network planning relies on Compound Annual Growth Rate (CAGR). However, applying the same growth estimate across the entire network is not always accurate due to various factors such as economic, social, or demographic reasons. For example, a community with a nearby university is expected to have a different traffic behaviour during the school year compared to the summer, and a community that hosts major sports franchises exhibits higher traffic depending on regular and post-season performance. 

Incorrect growth estimates can result in premature investments at different locations. Also, one can miss important network burst patterns based on high profile events such as smart phone updates, major video game releases or live global sporting events (e.g. the 2022 FIFA World Cup). Attempts were made to address these shortcomings by splitting the network into smaller chunks, and then manually analyzing growth expectations. The granularity and manual labor required to produce useful results made this approach unworkable as you scale the analysis. A new method is required for better traffic forecasting that will allow for targeted and timely spending.

This paper proposes a traffic forecasting approach that shows how Machine Learning (ML) can be used to automate iterative calculations and model attributes such as trends and seasonality, failure events along with subsequent interactions between the primary and failover links, and network burst patterns. Our predictive models have the computational power to scale the analysis of the multiple variables and high granularity. This proposal is a powerful and repeatable capacity-planning strategy that enables targeted network augmentation and spending.

##### Tools: 

### C.2 Covid-19 Lockdown and Pollution in the City of Chicago

[streamlit](https://dianemads-capstone-streamlitstreamlit-hyz5lm.streamlit.app/)

[github](https://github.com/dianeMADS/capstone)

For this project, we explored the Chicago Array of Things (AoT) Dataset. This massive dataset was collected between 2018 and 2020 from a node array installed throughout the city of Chicago. Nodes have a variety of sensors installed at each location. These sensors fall into one of six categories air quality, meteorological, physical, environmental, system, and vision. Initially, we hoped to focus on determining the quality of life around the city. This proved to be a bit too ambitious, however. We found it very difficult to define quality of life and focus in on key measurements. Instead, we focus mainly on the air quality metrics. These metrics are easier to track over time and there are clear definitions for gas concentrations that are considered dangerous or unhealthy. The analysis focuses on the concentrations of five gasses: CO, H2S, NO2, O3, and SO2, as well as oxidizing and reducing gas concentrations.

##### Tools: 

### C.3 Cryptocurrency Analysis

[pdf](https://github.com/dianeMADS/milestone2/tree/main/report/)

[streamlit](https://dianemads-milestone2-i4rryagqxtyey26mafg5eb.streamlit.app/)

[github](https://github.com/dianeMADS/milestone2)

For our Milestone 2 project we had two tasks, supervised learning and unsupervised learning analysis. We decided to try to do next-day price prediction for the supervised learning part because it was a simpler goal for us to understand. For the unsupervised learning part of the project, we wanted to see if we could find families of coins whose prices tend to move together. This was accomplished by finding similar price movement through dynamic time warping and clustering, with the result being quite reasonable.

For data collection, we used Coinmetrics and LunarCrush, which cover over a thousand cryptocurrencies providing real-time, daily & weekly updates and historical data, regarding market volume, market capitalization, transactions, coins in wallet, social media data, etc. Coinmetrics archives cryptocurrencies since January 2010, meaning data are available almost from creation for almost all existing coins. LunarCrush makes available the last two years worth of data, mostly having to do with social media. Both Coinmetrics and LunarCrush provide free APIs that facilitate historical data downloading.

##### Tools: 

### C.4 NBA

# D. Self-Learning
D.1 Data Manipulation
