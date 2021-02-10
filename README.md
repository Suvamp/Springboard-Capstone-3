# Springboard-Capstone-3
## **COVID-19 Time Series Analysis & Forecasting**

The current pandemic caused by the COVID-19 virus has affected the socioeconomic circumstances of numerous people globally. The purpose of this project will be to analyze the time series and forecast outcomes of the pandemic.

![](Capstone%203%20(Modeling)/Geographical%20Scatterplot.PNG)

### **1. Data**

The Johns Hopkins dataset from Kaggle. This dataset is real and is curated from several different, notable health organizations such as WHO, ECDC, and US CDC. This dataset has daily level information on the number of affected cases, deaths and recovery from 2019 novel coronavirus. Also, this is a time series data and so the number of cases on any given day is the cumulative number. The data is available from 22 Jan, 2020 and goes on till 09/23/2020.

> * [Kaggle](https://www.kaggle.com/sudalairajkumar/novel-corona-virus-2019-dataset)

### **2. Data Wrangling**

* I explored the data to see the type of data for each column, the size of the data, and checked the dataset for missing values. The dataset contains a total of 116805 entries and 7 columns. Overall, there are no missing values other than the Province/State column. This can be due to several factors such as the country not having any provinces or data being recorded for the entire country. For this project, I am just focusing on the data from each country, so it is a good sign that the other columns are not missing any values.
* To start off, I dropped columns which were not necessary, such as ‘Province/State’, ‘Last Updated’, and ‘Sno’. Furthermore, I uploaded a population dataset which had the population for each country. I renamed a few countries in the covid dataset in order for a smooth merge with the population dataset. The population dataset is being used to understand the severity of the covid virus in each country. Just seeing which country has the most number of cases or deaths is not a very efficient way of understanding the data. For a better analysis, the number of cases, deaths, and recovered will be divided by the population, to see which country has the highest density in each case.
* The dataset was also checked for duplicate values.
* Also, there a whole lot of datasets which were used for analysis. There is an entire dataset which records the number of cases and deaths for US counties. 
* After all the data wrangling, the updated dataset was saved for EDA.

### **3. EDA**

* The EDA portion is one of the largest portions of this project due to the variety of datasets provided by Johns Hopkins University. This section analyzes global data and US states data.
* **Step 1:** Created Time Series Plots to visualize the Top 10 countries with the most confirmed, deaths, and recovered.

![](Capstone%203%20(EDA)/Time%20Series%20of%20Top%2010%20Confirmed.PNG)

![](Capstone%203%20(EDA)/Time%20Series%20of%20Top%2010%20Deaths.PNG)

![](Capstone%203%20(EDA)/Time%20Series%20of%20Top%2010%20Recovered.PNG)

* **Step 2:**  Created Choroplethmaps and ranking for all the cases (confirmed, recovered, deaths, active) and their density globally.

  > **Confirmed**
  ![](Capstone%203%20(EDA)/Choropleth%20map%20of%20confirmed.PNG)

  ![](Capstone%203%20(EDA)/Rank%20map%20of%20confirmed.PNG)
  
  ** **Confirmed per Million**
  ![](Capstone%203%20(EDA)/Choropleth%20map%20of%20confirmed%20per%20million.PNG)
  
  ![](Capstone%203%20(EDA)/Rank%20map%20of%20confirmed%20per%20million.PNG)
  
  ** **Deaths**
  ![](Capstone%203%20(EDA)/Choropleth%20map%20of%20deaths.PNG)
  
  ![](Capstone%203%20(EDA)/Rank%20map%20of%20deaths.PNG)
  
  ** **Deaths per Million**
  ![](Capstone%203%20(EDA)/Choropleth%20map%20of%20deaths%20per%20million.PNG)
  
  ![](Capstone%203%20(EDA)/Rank%20map%20of%20deaths%20per%20million.PNG)
  
  ** **Recovered**
  ![](Capstone%203%20(EDA)/Choropleth%20map%20of%20recovered.PNG)
  
  ![](Capstone%203%20(EDA)/Rank%20map%20of%20recovered.PNG)
  
  ** **Recovered per Million**
  
  ** **Active**
  
  ** **Active per Million**
