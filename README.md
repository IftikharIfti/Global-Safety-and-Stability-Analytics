# Tableau Analytics Dashboard

## Motivation for the project:
Before doing this project I was surfing the internet which countries are best to live. Usually people tend to choose only those countries which are economically stronger such as high GDP per capita. But high GDP per capita doesn't always ensure a better place to live in. There are lists where it shows living index which doesn't say perfectly which factors were considered to make the list. So, I have made my own index analysis. It takes account on different other indexes and combine them to get an overall result. The factors I have considered:      
* Global Peace Index
* Global Health Index
* Global Crime Index
* Global Homicide Justice Rate
* Global Militarisation Index
* 

## Preview of the analytics dashboard:
![Image](https://github.com/user-attachments/assets/5dd88beb-b3b5-47b7-b8eb-d0e0dcf0c686)


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
