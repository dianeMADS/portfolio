This presents examples of data science projects completed by for work, academic, and self-learning purposes. They include some dashboards developed to support leadership and engineers in decision-making, and a few analysis involving machine learning for predictive modelling and clustering.

<!-- This webpage provides examples of data science projects completed by Diane for work, academic, and self-learning purposes. Those studies encompasses a broad range of skills including: 
- RESEARCH SKILLS: critical thinking; qualitative inquiry; study design (questions, hypothesis, methodology); technical writing; oral presentation to both leadership and technical audiences
- METHODS: web scraping, databases and cloud computing; data wrangling and data manipulation; visualization and dashboarding; statistical analysis; data mining and machine learning for causal inference analysis, network and social media analysis, learning analysis, and NLP
- TOOLSET: SQL and key-value NoSQL; Python programming for data analysis; AWS cloud computing (SageMaker, S3, Athena); SnowFlake; Alteryx; Tableau; Power BI
<br>
-->

# A. Dashboards
The context for this set of dashboards is a service provider network with millions of users and a mix of all types of internet traffic. The network has hundreds of links with varied capacities, from multiple 10Gs for smaller hubsites to tens of 100Gs for backbone links. Link costs are also varied as some are on the service provider's own fiber infrastructure while others are leases from other providers.

One visualization is to give leadership a high-level view of the network topology and bandwidth utilization. Giving network state at specific times, especially under critical conditions, facilitates discussions on growth requirements and network expansions. 
Other dashboards comprise congestion and failover tables, historical trends, and resource availability reports, equipping network engineers with tools assisting in decision-making for network resource planning.
###### Main Tools: SQL, AWS (Athena & S3), Alteryx, SnowFlake, Tableau

[Please follow the link to dashboards](https://dianemads.github.io/dashboards/)

<!-- Please click on the title to browse through a few examples of dashboards developed for various audiences including leadership, engineering and operations of an ISP. 
##### Tools: SQL, AWS Athena & S3, Alteryx, SnowFlake, Tableau
<br>
-->

# B. Data Analytics
## B.1 Leveraging Machine Learning for Network Traffic Forecasting
This study showing how machine learning could be leveraged to improve accuracy in growth estimates and enable targeted network augmentation (using trends, seasonality and traffic patterns), received a presentation opportunity at the SCTE conference in October 2023.

#### Abstract
Traditional network planning relies on Compound Annual Growth Rate (CAGR). However, applying the same growth estimate across the entire network is not always accurate due to various factors such as economic, social, or demographic reasons. For example, a community with a nearby university is expected to have a different traffic behaviour during the school year compared to the summer, and a community that hosts major sports franchises exhibits higher traffic depending on regular and post-season performance.

Incorrect growth estimates can result in premature investments at different locations. Also, one can miss important network burst patterns based on high profile events such as smart phone updates, major video game releases or live global sporting events (e.g. the 2022 FIFA World Cup). Attempts were made to address these shortcomings by splitting the network into smaller chunks, and then manually analyzing growth expectations. The granularity and manual labor required to produce useful results made this approach unworkable as you scale the analysis. A new method is required for better traffic forecasting that will allow for targeted and timely spending.

This paper proposes a traffic forecasting approach that shows how Machine Learning (ML) can be used to automate iterative calculations and model attributes such as trends and seasonality, failure events along with subsequent interactions between the primary and failover links, and network burst patterns. Our predictive models have the computational power to scale the analysis of the multiple variables and high granularity. This proposal is a powerful and repeatable capacity-planning strategy that enables targeted network augmentation and spending.

###### Methods and Tools: linear and exponential regressions, advanced time series forecasting models (STL, Holt-Winters Exponential Smoothing, ARIMA, LSTM), AWS (SageMaker & S3), SQL, Python (Pandas, NumPy, Math, Matplotlib, Seaborn, statsmodels, pmdarima, Scikit-learn, Keras & TensorFlow)

[D.P. Onguetou, A. Maddumabandara and J. Lee, Leveraging Machine Learning for Network Traffic Forecasting, Proc. of the <em>Society of Cable Telecommunications Engineers (SCTE) Technical Forum</em>, Fall 2023.](https://www.nctatechnicalpapers.com/Paper/2023/3580_Lee_5100_paper)
- <a href="https://github.com/dianeMADS/traffic-forecasting/blob/main/assets/3580_DPO_5100_presentation.pdf">Presentation</a> 

<!-- [github](https://github.com/dianeMADS/traffic-forecasting/tree/main)
-->

## B.2 Covid-19 Lockdown and Pollution in the City of Chicago
This analysis was completed in December 2021, as part of requirements for the Master of Applied Data Science degree at the University of Michigan. 

We chose to explore  the [Chicago Array of Things (AoT) dataset](http://arrayofthings.github.io/). This massive dataset was collected between 2018 and 2020 from a node array installed throughout the city of Chicago. Nodes have a variety of sensors installed at each location. These sensors fall into one of six categories air quality, meteorological, physical, environmental, system, and vision. Initially, we hoped to focus on determining the quality of life around the city. This proved to be a bit too ambitious, however. We found it very difficult to define quality of life based on available measurements. Instead, we focused mainly on the air quality metrics. These metrics are easier to track over time and there are clear definitions for gas concentrations that are considered dangerous or unhealthy. The analysis focuses on the concentrations of five gasses: CO, H2S, NO2, O3, and SO2, as well as oxidizing and reducing gas concentrations.

###### Methods and Tools: causal inference analysis, vector autoregression, clustering, Google colab, Python (Pandas, NumPy, Math, Matplotlib, Seaborn, statsmodels, folium, altair, gzip, os), C++

- [Blog](https://dianemads-capstone-streamlitstreamlit-hyz5lm.streamlit.app/)
- [Short video explanation](https://drive.google.com/file/d/13i5_bAYNkdLmUPxKhUNY_RBTNTcorssL/view?usp=sharing)
- [Guided tour for causal inference analysis](https://colab.research.google.com/drive/1d4nclhPZjrF58zoMY0_WiKBNh8j3n16a?usp=sharing)
- [Guided tour for clustering analysis](https://colab.research.google.com/drive/1cOF5HxLqgX7ctv5Kh9x1HmH6RCngOZdk?usp=sharing)
- [GitHub repository](https://github.com/dianeMADS/capstone)

## B.3 Cryptocurrency Analysis
This project was another requirement for University of Michigan Master of Applied Data Science degree, completed in September 2021. There were two mandates: supervised learning and unsupervised learning analysis. We selected Coinmetrics and LunarChrush, which cover a thousand cryptocurrencies providing real-time, daily and weekly updates, as well as historical data. Coinmetrics archives cryptocurrencies since January 2010, meaning data are available from the creation of almost all existing coins, while LunarCrush makes sentiment-like social media data available since September 2019. Both Coinmetrics and LunarCrush provide free APIs that facilitate data downloading. Knowing little about cryptocurrency, we decided to try to do next-day price prediction for the supervised learning part because it was a simpler goal for us to understand. For the unsupervised learning part of the project, we wanted to see if we could find families of coins whose prices tend to move together. This was accomplished by finding similar price movement through dynamic time warping and clustering, with the result being quite reasonable.

###### Methods and Tools: LSTM, Random Forest, Clustering, Deepnote, Python (Pandas, NumPy, SciPy, Scikit-learn, TensorFlow, Altair, Malplotlib)

- [Final Report](https://github.com/dianeMADS/milestone2/blob/main/report/MADS-milestone2-Onguetou-Nikolsky.pdf)
- [Further visualizations](https://dianemads-milestone2-i4rryagqxtyey26mafg5eb.streamlit.app/)
- [GitHub repository with source codes](https://github.com/dianeMADS/milestone2)
<br>

## B.4 Path to the NBA: a detailed look into ESPN High School Basketball Player ratings predictability on making it to the NBA, May 2021
This project the first milestone of the Master of Applied Data Science degree at the University of Michigan. The objective was to demonstrate mastering data collection and manipulation, and statistical analysis. Through the analysis, we determined how effective is ESPN's high school basketball rankings at predicting whether a player eventually gets drafted into the league. We also tried to specify characteristics that top players have in common that make it to the NBA, and how many years is necessary on average to get drafted.

###### Methods and Tools: web scraping, KNN, Jupyter notebook, Python (pandas, numpy, requests, matplotlib, plotly, seaborn, scipy, altair, scikit-learn)

- <a href="https://github.com/dianeMADS/milestone1/blob/main/ESPN-to-NBA%20vFinal-1.pdf">Presentation</a>
- [GitHub repository with notebook](https://github.com/dianeMADS/milestone1)

[//]: # (# D. Self-Learning)
[//]: # (D.1 Data Manipulation)
