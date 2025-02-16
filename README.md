# Global Safety and Stability Analytics

## Motivation for the project:
Before doing this project I was surfing the internet which countries are best to live. Usually people tend to choose only those countries which are economically stronger such as high GDP per capita. But high GDP per capita doesn't always ensure a better place to live in. There are lists where it shows living index which doesn't say perfectly which factors were considered to make the list. So, I have made my own index analysis. It takes account on different other indexes and combine them to get an overall result. The factors I have considered:      
* [Global Safety Index](https://www.visionofhumanity.org/maps/#/)
* [Global Health Index](https://www.numbeo.com/health-care/rankings_by_country.jsp)
* [Global Crime Index](https://www.numbeo.com/crime/rankings_by_country.jsp)
* [Global Homicide Justice Rate](https://dataunodc.un.org/dp-intentional-homicide-victims)
* [Global Militarisation Index](https://gmi.bicc.de/ranking-table)
* [Global Press Freedom Index](https://rsf.org/en/index)
* [GDP Per Capita](https://wits.worldbank.org/CountryProfile/en/Country/BY-COUNTRY/StartYear/2010/EndYear/2022/Indicator/NY-GDP-PCAP-CD)         
These were factors I took into consideration in making my final index which is the Global Safety and Stability index.
## Calculation Method:
* First I scrapped all these indexes from the respected websites. I took all the available years
* I aligned all the indexes within same range 0 to 1 fr
* Then I took only those countries which were available in all of the indexes
* For years I took the lowest maximum year and highest minimum year
* In the final list only 71 country was present and the year range was from 2013 to 2021
* Then I multiplied each index with 1/6 and then added all of them

## Preview of the analytics dashboard:
![Image](https://github.com/user-attachments/assets/5dd88beb-b3b5-47b7-b8eb-d0e0dcf0c686)

## Findings From the index:
* Estonia was consistence in safety and stability index throughtout 2013 to 2021 even though its GDP per capita is around 20000 USD.
* Most of the countries are from Europe. Only two asian countries, Singapore and Japan were able to stay in top 15
* Other than Singapore and Japan  Saudi Arabia, Turkemenistan, Armenia were also close to the top countries
* Powerful countries like China, Russia, India fell behind due to poor infrastructure in other domains.
* Higher GDP per capita doesn't mean better safety and stability. Ireland having highest GDP per capita in 2021 still were unable to stay in top position. This is due to less focus in important fields such as militarisation, Health. Countries like United States, Canada are also behind despite having high GDP per capita.
* But if we look carefully and consider 0.6 as good threshold, most of the high GDP per capita countries were able to stay there.
* So, the conclusion can be like this: high GDP per capita doesn't ensure safety and stability but a country prosper if their economy is strong enough

## Steps to run the project

1. First clone the repository:
```bash
git clone https://github.com/IftikharIfti/Global-Safety-and-Stability-Analytics.git
```
2. Then install the dependencies given in requirements.txt file
```bash
pip install -r requirements.txt   
```
3. Download the latest Chromedriver from Google. Please check if the chromedriver version matches with your chrome browser version.
4. Then first run all the ipynb file of Web Scrapping
5. After that, run all the files of Data Preprocessing except Global Homicide Justice Index.ipynb. After running all other files, then run this Global Homicide Justice Index.ipynb file
6. Lastly go to Index Combination folder to combine all my index by running Global Safety and Stability Index.ipynb file and create a new index called Global Safety and Stability index
7. Getting the necessary excel files then I have proceeded to create data visualization in tableau

Tableau Public View:
https://public.tableau.com/app/profile/iftikhar.jaman.ifti/viz/GlobalSafetyandStabilityIndexTrends/Dashboard1?publish=yes
