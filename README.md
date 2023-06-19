**Housing in GTA** <br />
Project Introduction:(required)<br />
What factors contribute to housing prices within the different regions of GTA?<br />
People always consider buying a house as an excellent investment. And the GTA housing market has always been optimistic, even during COVID. But with the burgeoning population, people are worried about affordable housing. The following general questions come to mind:<br />
How population density is influencing dwelling numbers?<br />
Are housing supplies and demands in balance?<br />
Can school ranking affect housing prices?<br /><br />

This research project will focus on the GTA area, including Durham, York, Toronto, Peel, and Halton regions. The key points to be investigated upon are as follows: <br />
Population density with dwelling numbers<br />
Housing demands<br />
Housing supplies<br />
School ranking and housing choice<br />

Data Source:(not required in README)<br /><br />
Census 2021  Population and Dwellings https://data.peelregion.ca/datasets/RegionofPeel::census-2021-cd-csd-population-and-dwellings/about 
GTA Housing price between 2018-2021
https://trreb.ca/index.php/market-news/mls-home-price-index/mls-home-price-index-archive
GTA Elementary school ranking 2018-2020
https://www.fraserinstitute.org/sites/default/files/ontario-secondary-school-rankings-2018.pdf
https://www.fraserinstitute.org/sites/default/files/ontario-elementary-school-rankings-2019-12659.pdf
https://www.fraserinstitute.org/sites/default/files/ontario-elementary-school-rankings-2020-13385.pdf
GTA region
https://www.ureachtoronto.ca/city-services/
Data Cleaning:(required)
For the GTA Census 2021 data, the csv file was downloaded from the source website. 
The GTA housing price was downloaded as a PDF file by month in different years, then we manually cleaned the data into a csv file.  
GTA School Ranking data was download in csv file by year from the data source 
We used Pandas to clean and format all the datasets. We have created multiple Jupyter Notebooks for data exploration and cleanup processes. All raw data files, and cleaned datasets are stored in this repository separately. Moreover,  all presentation distributed graphs have been saved in this repository separately as well.<br />
**Key Findings:(required)** <br /><br />
By analysing Census 2021 data, we see that the population and the dwellings numbers in GTA have both grown. From comparing the Census 2016 data, we could see the dwelling percentage change is higher than the population percentage change in Toronto, York, and Peel. When excluding public dwellings, and counting in population density, we could see that population density and private dwelling numbers are in a positive relationship. <br /><br />
The housing prices have been increasing through 2018-2021, but the housing prices in Toronto, York, Halton has dropped in 2020. With COVID work-from-home policy, we could see people have taken this opportunity to pursue cheaper housing. Based on the analysis of the average sold price and the number of houses sold in each month of 2021, we draw a graph to understand the relationship between housing supplies and demand. It showed that the equilibrium point between housing supplies and demands is 14,007 sold houses with the average price of $989,172. The data is showing the housing market is a seller’s market. For all the points, that are above the equilibrium point, means the housing market is in excess supply.<br /><br />

Since it was going to be costly to get a more accurate data for housing demand, we ended up measuring it based on the number of houses sold per month. After aggregating   	 the sum for each year and each region, we found that the demand did increase each year except for 2019 where it dropped by 3.42%. However, from 2018-2021 we did see an overall increase of 36.34%. The drop in 2019 could be due to the raising in prime interest rate of 3.70% July 2018 to 3.95% in January 2019. In addition, there were a lot of talks in the news about housing bubbles where the hype in demand was causing housing prices to inflate. The two regions that were not affected in 2019 were Durham and York region. These 2 regions followed the price increase trend. Based on the regression analysis, the correlation between the demand and average house price is 0.42. This indicates that there is a positive moderate relationship between the 2. The maximum demand is 33,182 houses and the minimum is 559 houses. The median is 2898 houses. Looking at the scatter plot graph, the majority of the data is clustered between 600 to 4500 range. The outliers are contributing to the weaker r-squared and correlation value.<br /><br />
 
Shifting to supply, we measured it based on the new numbers of listings per month, but not the ones that were actively listed. In 2020, supply continued to increase except for the York and Durham region. Once York region was the only one that continued to follow the average price trend. The increase of housing on the market for Toronto was partially due to Covid. Many people saw an opportunity to move out of the city since working from home felt permanent. In the GTA, some people saw that it was an opportunity to move into Toronto due to the dip in price. From 2018 to 2021, we saw an overall increase of 33.77%. One thing to note, in 2020 Peel Region, the housing price did dip, but the supply continued to increase, whereas Durham region did the opposite. The housing prices continued to increase, but the supply did drop. The regression analysis does show a very similar trend to demand. The correlation coefficient is 0.44 and r-squared is 0.2. We ended up using the same average house price as demand since it is somewhat known that the listing price of the house on the market is purposely set low to attract buyers and create bidding wars to generate more profit. As a result it creates a sense of strong demand for houses.<br /><br />

Turning to the supply and demand curve for 2021, the equilibrium point is at 14,007 houses at an average price point of $989,172. To generate both curves/lines, we took the max and min point for both supply and demand and created the same size array to plot the lines on the graph. Based on the equation to determine if it is a buyer’s or seller’s market, we can see that it is a buyer’s market, since the quotient clearly demonstrates that the supply is nowhere near 5 times the size of demand. However, if the quotient is greater than 7, it would be a buyer’s market. In addition, the data supports a surplus in the market, as the average price sits around $1.1M. This indicates that there are affordability issues rather than a shortage in the market. <br /><br />

One factor we assumed will affect housing prices in GTA is school ranking. From the available data, we compiled elementary school ranking distributions between 2018 to 2020 in GTA. The overall area-wise ranking distributions were quite similar over the years. The consistent best rankings were observed in the Halton and the York regions while the poorer rankings were observed in the Toronto, Peel and Durham regions. A correlation test between the area-wise housing prices and the corresponding school rankings showed a very weak negative correlation over the years. It could indicate that elementary school rankings may not have an effect on the housing market. However, we found that housing price, sales volume and school ranking all have wider distributions in the Toronto, Peel and Durham regions generating a large number of outliers. This could have affected the correlations. Finally, conducting a trend analysis combining area-wise school ranking, sale price and sale volume, we find that there is a greater preference for purchasing houses in the Toronto, Peel and Durham regions, despite them having lower school rankings.<br /><br />

In conclusion, we would highlight that the most important contributing factors to housing prices are population growth and regional demands. School ranking is one attribute among the regional demands. Our research suggests that there could be other contributing factors, such as proximity to amenities, employment opportunities, or access to culture and communities, for the rising housing prices. <br /><br />

Team Member:(required)
Darvy Teav
Arefin Shamsil
Wei Zhang
![dwelling_density](https://github.com/Dav5T/Grp-Project-1---Housing-Price/assets/130593953/10fbe366-3c4e-4632-a210-1017435a6694)

![Private_dwellings_by_residents](https://github.com/Dav5T/Grp-Project-1---Housing-Price/assets/130593953/615f5850-d7f8-4f29-a999-bad73f2b7e7c)

![Average_price_per_year](https://github.com/Dav5T/Grp-Project-1---Housing-Price/assets/130593953/3772e076-ad2f-485b-981c-278c693effde)

![Average_price_per_Region](https://github.com/Dav5T/Grp-Project-1---Housing-Price/assets/130593953/9080ccc4-16e3-494b-936e-d527f67d127c)

![GTA_Map_Price_2021](https://github.com/Dav5T/Grp-Project-1---Housing-Price/assets/130593953/4f783ed0-e010-4860-9af4-23fc633118b7)

![Demand_per_Region](https://github.com/Dav5T/Grp-Project-1---Housing-Price/assets/130593953/7af30d8b-9a23-4279-91df-443b219ddfcd)

![Demand_per_year](https://github.com/Dav5T/Grp-Project-1---Housing-Price/assets/130593953/454ab26e-869d-4f01-bce4-bd2ec46e9678)

![Average_price_vs_demand](https://github.com/Dav5T/Grp-Project-1---Housing-Price/assets/130593953/9865375b-ead5-44c7-9eca-bad94481904a)

![Supply_per_region](https://github.com/Dav5T/Grp-Project-1---Housing-Price/assets/130593953/12b4b2d0-ede8-4dce-aaff-2cd0e285e1f3)

![Supply_per_year](https://github.com/Dav5T/Grp-Project-1---Housing-Price/assets/130593953/2391a30a-150d-42b8-ad12-5f1b6b792065)

![Average_price_vs_supply](https://github.com/Dav5T/Grp-Project-1---Housing-Price/assets/130593953/b07d4474-1cc0-4230-8b26-b5c85b2e1f82)

![Supply_Demand_Curve](https://github.com/Dav5T/Grp-Project-1---Housing-Price/assets/130593953/fcc4d36a-e047-4afe-9c47-8c08c8aa0279)

![Total_Supply_Demand](https://github.com/Dav5T/Grp-Project-1---Housing-Price/assets/130593953/b7c655de-cf7a-477a-9627-66430c2c5c7f)

![Fig - school score 2018](https://github.com/Dav5T/Grp-Project-1---Housing-Price/assets/130593953/c311731a-2e19-4df9-8199-df7ce1e66199)

![Fig - school score 2019](https://github.com/Dav5T/Grp-Project-1---Housing-Price/assets/130593953/1fbdbb7e-ff98-432e-9996-d9de628d8927)

![Fig - school score 2020](https://github.com/Dav5T/Grp-Project-1---Housing-Price/assets/130593953/ea90fcc4-6038-4547-84f1-c6f9f48f75a4)

![School-price-sales](https://github.com/Dav5T/Grp-Project-1---Housing-Price/assets/130593953/a0b0fa6c-aacf-4243-a3a1-53aaff841429)




