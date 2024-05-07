# Mathematical-Modeling
Solving for 2023 APMCM mathematical modeling contest Problem C.  
Our paper: [Capmcm2305738.pdf](https://github.com/Capa4566/mathematical-modeling/files/15231726/Capmcm2305738.pdf)

## Problems we solved by building mathematical models

1. Analyze the main factors affecting the development of new energy electric vehicles in China.
2. Predict the development of China’s new energy electric vehicles in the next 10 years.
3. Analyze the impact of new energy electric vehicles on the global traditional energy vehicle industry.
4. Analyze the effects of the policies targeted to resist the development of new energy electric vehicles in China.
5. Analyze the impact of the electrification of new energy electric vehicles (including electric buses) in cities on the ecological environment

## Problem 1
In order to analyze the main factors that affect the development trend of new energy electric vehicles in China, we can leverage the Grey relational analysis (GRA) model. GRA is well-suited for studying the intricate relationship among different factors influencing the development of new energy electric vehicles (NEEVs) in China. To ensure the effective application of the GRA model, our initial undertaking revolves around the identification and systematic collection of data spanning from 2013 to 2022. We have compiled a comprehensive dataset encompassing various aspects such as electric vehicle performance, technological advancements and economic conditions for our research. By quantifying the degree of relevance of each factors using GRA model, we are able to obtain that the NEEVs sales is the most relevant to the development of NEEVs thus it can best indicate the development of NEEVs in China. Following the sales, the NEEVs ownership, energy efficiency and number of charging piles are also highly relevant to the NEEVs development.  

**Solution of GRA Model:**  
<div align=center><img width="550" height="350" src="https://github.com/Capa4566/mathematical-modeling/assets/96423522/27e6f6ee-1c30-4765-a103-078316342fab"/></div>  
  According to the above figure, we can observe the correlation trends of seven indicators influencing the development of new energy vehicles from 2013 to 2022. In order to form a more intuitive orrelation   sequence, we calculated the average values of each factor across different dimensions, and the sorted results are shown in the table below:  
<div align=center><img width="500" height="250" src="https://github.com/Capa4566/mathematical-modeling/assets/96423522/1e2a0ce1-b17b-48f9-83cc-ec55396cac22"/></div>  
  Based on the degree of relevance, we can conclude that the sales factor has the highest correlation with the development of NEEVs in China following by the NEEVs Ownership, Energy Efficiency of NEEVs and   the Number of Charging Piles with 0.87 degree of relevance. Therefore, we can state that these 4 factors are the main factors affecting the development of NEEVs and that by making improvements on these     factors should results in significant impact on the development of NEEVs in China.
  

## Problem 2
To predict the future development trends of China's new energy vehicles over the next 10 years, we utilize historical data as the foundation to establish an ARIMA model for forecasting. We collected 13 factors affecting the NEEVs industry development from year 2013 to 2022 and among them, we selected 6 indicators to predict the development of China's NEEV in the next 10 years. The 6 indicators are the number of NEEVs patent applications, NEEVs market penetration rate, NEEVs production, NEEVs ownership in China, charging cost and the number of charging piles. By using the ARIMA model, we are able to forecast the development of the 6 indicators from 2023 to 2032.  

**Establishing ARIMA model:**   
The Autoregressive Integrated Moving Average (ARIMA） model is a popular and widely used statistical analysis method for time series data forecasting. ARIMA model combines the concepts of AutoRegressive (AR), Integrated (I), and Moving Average (MA), enabling the handling of non-stationary time series and transforming them into stationary ones. In the ARIMA model, denoted as ARIMA(p,d,q):  
<div align=center><img width="1000" height="40" src="https://github.com/Capa4566/mathematical-modeling/assets/96423522/c71397ec-11f6-4492-94d1-7175f495954a"/></div>  
The basic idea of the ARIMA model is to adjust the values of the three parameters, p, d, and q to better fit historical data and enable predictions for the future.

   <br/>**Solution of ARIMA model:**   
As results of the ARIMA model, we depict the prediction of NEEVs development in China from 2023 to 2032 in the form of graph together with the existing data from 2013 to 2022 for better visualization of the development trends.  
<div align=center><img width="550" height="350" src="https://github.com/Capa4566/mathematical-modeling/assets/96423522/b9dd6fc0-f0ff-4189-8c29-c636261f009e"/></div>   <br/>
<div align=center><img width="950" height="750" src="https://github.com/Capa4566/mathematical-modeling/assets/96423522/9ac14c4c-f8cb-4a69-a5b3-066979c85c34"/></div>  

  
## Problem 3 and Problem 4
We leverage the same model to solve question 3 and question 4. Question 3 involves analyzing the impact of new energy electric vehicles (NEEVs) on the global traditional energy vehicle industry. Question 4 explores the effects of policies implemented by other countries to resist the development of NEEVs in China. Since both of these questions aim to quantitatively analyze the correlation relationships, we utilize Linear Regression to establish the model. For Question 3,we get the results. For Question 4, We compare the growth rate and number of NEEVs exported by China to the other countries before and after the implementation of the policy.  

**Establishing Linear Regression model:**   <br/>
We simplify the issue by considering a linear model that encompasses multiple influencing factors. Assuming the primary factors affecting the development of new energy electric vehicles are government policies, economic, market demand, technological advancement, etc., we can utilize the following linear model:
<div align=center><img width="500" height="70" src="https://github.com/Capa4566/mathematical-modeling/assets/96423522/fc3f3bdf-814a-46b7-8058-ee0b1c7604cb"/></div>  
For Question 3, we let the global traditional car sales be Y. The coefficients β0, β1, β2, β3, β4 in the model represent the effect of the corresponding variable, such as policy,,market demand and technological advancement to the development of NEEVs. 𝛼 ∑4 𝑖=1 𝛽𝑖2 is the different of model.  
Lasso regression:  
<div align=center><img width="500" height="100" src="https://github.com/Capa4566/mathematical-modeling/assets/96423522/1668ee42-15d0-440f-a893-909a85066d09"/></div>    
  
**Solution of Linear Regression model:**   

For Problem 3:  
<div align=center><img width="550" height="350" src="https://github.com/Capa4566/mathematical-modeling/assets/96423522/8e5a2171-4b57-45f8-8bbe-59cfde998175"/></div>  
Referring to the above figure, we can conclude that the linear regression model in question three can make predictions about the global conventional car sales changes based on indicators influencing the development of NEEVs. Moreover, the predicted results exhibit a similar trend to the actual sales. Therefore, we can infer that with the development of NEEVs, global conventional car sales have experienced significant fluctuations since 2018, with a noticeable decline in sales.   <br/>

   <br/>For Problem 4:      
When not considering the resistance policy, the average sales growth rate of NEEVs in EU countries and the average sales growth rate of NEEVs in China are as follows:  
<div align=center><img width="750" height="400" src="https://github.com/Capa4566/mathematical-modeling/assets/96423522/dfa35dc7-56b8-4c7c-b51c-5c75d1416f7c"/></div>  
After incorporating the resistance policy into the model, we predict the sales growth rate of global NEEVs to be:  
<div align=center><img width="550" height="350" src="https://github.com/Capa4566/mathematical-modeling/assets/96423522/96c2f33a-38a4-4f48-a70a-ca0d203e4405"/></div>  
And the global sales of NEEVs considering the resistance policy indicator and the sales of NEEVs in China without considering the boycott policy indicator are:  
<div align=center><img width="750" height="400" src="https://github.com/Capa4566/mathematical-modeling/assets/96423522/9206c71b-ff6e-4700-a1aa-42dbcd723299"/></div>    

  
## Problem 5  
We collected population data for cities with populations exceeding 1 million in various countries, along with data on carbon emissions, emissions of four automobile exhaust pollutants, and the ownership of new energy vehicles (NEEVs) and electric vehicles. Through data analysis, we aim to correlate the relationship between population and ownership, the relationship between carbon emissions and pollutant emissions, and how these two relationships mutually influence each other. By doing so, we can predict the impact of different scales of new energy vehicles on carbon emissions and pollutant emissions when a city's population reaches 1 million.   <br/>

**Establishing Green Vehicle Popularization and Environmental Impact Model:**  
The following formula is used to calculate the proportion of energy vehicles in various categories.  
Ratios Calculation:  
<div align=center><img width="500" height="100" src="https://github.com/Capa4566/mathematical-modeling/assets/96423522/640717a2-04b0-4e59-98de-f7686a0bbabf"/></div>  
<div align=center><img width="500" height="145" src="https://github.com/Capa4566/mathematical-modeling/assets/96423522/40e478e3-77f0-4f7f-b91d-2be9b830e25a"/></div>  
Calculation of 𝐶𝑂2 Emissions per Unit GDP:  
<div align=center><img width="450" height="60" src="https://github.com/Capa4566/mathematical-modeling/assets/96423522/ac31c8aa-4307-40c0-82b7-91e9d7fb3fd3"/></div>  
This equation is used to evaluate the impact of economic activities on 𝐶𝑂2emissions in a country or region. This formula calculates the 𝐶𝑂2emissions (𝐶𝑂2Emissions) per unit of population (Population) in millions (1,000,000 units).  
Calculation of Total Emissions of Four Pollutants:  
<div align=center><img width="450" height="40" src="https://github.com/Capa4566/mathematical-modeling/assets/96423522/6e12499d-b53f-40ab-a4f4-75bfc22819eb"/></div>   
This formula represents the total emissions of four major pollutants (TotalEmissions), including Carbon Monoxide (CO), Volatile Organic Compounds (VOC), Nitrogen Oxides (NOx), and Particulate Matter (PM). Then, we compare the images based on the analysis output.     <br/>

   <br/>**Solution of Green Vehicle Popularization and Environmental Impact Model:**  
<div align=center><img width="750" height="550" src="https://github.com/Capa4566/mathematical-modeling/assets/96423522/a31b52e0-f8be-4235-abcd-438e9ee45599"/></div>  
<div align=center><img width="750" height="400" src="https://github.com/Capa4566/mathematical-modeling/assets/96423522/d61474da-6a34-4cf4-a948-0727fd0b5cd6"/></div>  

As depicted in the above figure, we estimated the ownership of New Energy Electric Vehicles (NEEVs) and pure electric vehicles in a city with a population of one million from 2015 to 2020. We also examined the impact of ownership on carbon emissions and exhaust pollutant emissions in the city. The results indicate that when the ownership of pure electric vehicles approaches that of NEEVs, meaning that a significant portion of NEEVs in the city are pure electric vehicles and the ownership is increasing annually, both carbon emissions and exhaust pollutant emissions in the city decrease over the same time series. Therefore, we can conclude that the electrification of NEEVs has a positive impact on the ecological environment of the city.
