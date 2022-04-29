# Play-store-app-review-analysis

### **Aim**- The Play Store apps data has enormous potential to drive app-making businesses to success. Actionable insights can be drawn for developers to work on and capture the Android market.

Analyze the data of 10841 apps available on play store. Each app (row) has values for catergory, rating, size, and more. Another dataset contains customer reviews of the android apps. Explore and analyze the data to discover key factors responsible for app engagement and success.


Our mobile play store is available with all type apps as it has enormous potential to drive any businesses to success. Thus, **actionable insights can be drawn for developers to work on and capture the Android market.**

In this project, through our exhaustive analysis of approx. 10k apps we discovered some key factors responsible for **app engagement** and its success. Initially we imported the required libraries such as numpy, pandas, matplotlib and seaborn to analyze the data and then read the csv file in Google Colab notebook given to us related to play store app review. Here we found that there are two sets of data i.e play store app and user reviews, so we **explored** the columns of both datasets.


After having understand the columns, we started with **data cleaning** in which we looked for** duplicates, null and missing values** in our dataset. We found that there are 1465 nan values in rating and 1 nan value in content rating. Also looking at the datatypes, we found that only rating is numeric datatype while others are text. So, we initially removed all duplicates, then after removing all nan values we converted the required columns to numeric so that we can start with extracting some statistical points for data analysis. Also, we looked for special characters (, $ +) and letters (M k) in the Installs, Size, and Price columns to make our task easy. 


Once the data was cleaned, we **extracted the statistical values** of numeric data types using info method and then moved on for **data analysis**. For analysis, we thought of analyzing categories of apps, their genres, rating, review, price, install and size columns first as these are the major factors on which success of any app relies. So, while analyzing categories, we noted that among 33 unique app categories present in our dataset, apps related to **Games and Medical have the highest market prevalence** according to their ratings though there are greater number of apps related to family and tools as well.

Secondly, by using **histplot, pyplot and boxplot** we found that among 199 genres the number of installs is higher for Communication, Social and productivity genres whereas Tools, Entertainment, Education related genres have maximum number of apps among all genres. 

![image](https://user-images.githubusercontent.com/98693201/165893372-b03912f2-7a6b-419a-a801-5d65ff2d0a2a.png)
![image](https://user-images.githubusercontent.com/98693201/165893409-4b39ddae-4fa1-4e84-ae27-94eebfe74d92.png)
![image](https://user-images.githubusercontent.com/98693201/165893446-7868c694-659a-4a40-95cb-43cf00311482.png)
![image](https://user-images.githubusercontent.com/98693201/165893691-4142eede-bd70-43d4-8fbe-a0f66b7fd712.png)


Further, using multivariate pairplot and heatmap for correlation, we analyzed all KPIs mentioned above. We plotted 5x5 matrix of 'Rating', 'Reviews', 'Size', 'Installs' and 'Price'. From this plot we found that:

*  Users have paid more for lite and high rating apps.
*  Users have installed more apps of the ones having high reviews
*  Installs of app doesn't depends on Size.

After analyzing the first dataset, we moved to second one i.e user reviews dataset which contained three different columns such as sentiment, sentiment analysis and sentiment polarity. So, after exploring and cleaning this dataset we started analyzing it and found that users showed more positive sentiments for paid apps and were harsh while showing sentiments for free apps. 

![image](https://user-images.githubusercontent.com/98693201/165893493-1e42c3b1-40a5-4b5b-8eeb-86f63a8c62fe.png)
![image](https://user-images.githubusercontent.com/98693201/165893600-61a987fa-56cc-4d58-8b29-d6d336f87e5e.png)


Lastly, we merged the two given datasets and found that users gave maximum reviews for game category followed by family. Also, the positive and negative sentiments were highest for games category.
Thus, after exploring our datasets thoroughly and concluding the necessary points for the success of any app, our objective of the project was completed. By this analysis, we are sure that it will help the developers of any app to target in the right direction and make it profitable

### **References-**
[1] Statista, Number of available applications in the Google Play store from December 2009 to March 2019, https://www.statista.com/statistics/266210/number-of-available-applications-in-the-google-play-store/,Online: accessed 22 May 2019.

[2] Statista, Number of mobile app downloads worldwide in 2017, 2018 and
2020 (in billions), https://www.statista.com/statistics/271644/worldwide-free-and-paid-mobile-app-store-downloads/, Online: accessed 22 May 2019.

