# Play-Store-App-Analysis

dataset used is given in the following csv files (given in repo) : 
1. Play store data 
2. User Reviews

The aim of this project was to analyse the given data and derive some meaningful insights from it. 

Process :
cleaning data : 
* removing null values
* removing duplicates
* setting the data type of each column right
  1. removing '+' and converting the 'Installs' column to int 
  2. converting reviews column to int
  3. fixing size column (making all values in MB and turning it to float dtype)
  4. setting the dtype of price column right
  
Making Inferences : 

1. Distribution of apps by category
<img width="689" alt="image" src="https://user-images.githubusercontent.com/70737240/233855762-d2868f29-7452-4382-88e6-8485286ef0a4.png">
---
Conclusion - Family, Game and Tools arethose categories which have most number of apps
---
2. Average rating of apps (overall)
<img width="709" alt="image" src="https://user-images.githubusercontent.com/70737240/233856020-d56e0c1c-c6e7-43d1-90fc-ece249c392f5.png">
---
Conclusion - most apps are rated a little less than 4.5
---
3. looking closely at each category - distribution or ratings in each category
<img width="690" alt="image" src="https://user-images.githubusercontent.com/70737240/233856117-89d2562d-b4bf-4b3e-a7c6-c469cd188ebd.png">
---
Conclusion - BOOKS_AN_REFERENCE and HEALTH_AND_FITNESS have the highest rated apps
---
4. are lighter apps better rated?
<img width="725" alt="image" src="https://user-images.githubusercontent.com/70737240/233856180-09f91090-57ed-4363-a9b8-4a1f6936972d.png">
---
Conclusion - most apps lie in the range of 0-10MB range
           - most paid apps are light weight
---
5. visualising the distribution between price and ratings
<img width="696" alt="image" src="https://user-images.githubusercontent.com/70737240/233856321-aa17508d-e62c-4903-aaad-4377dfc29809.png">
---
Conclusion - most apps lie in 0-$20 range, but we notice some really expensive apps (they were removed as the next step)
---
6. distribution of paid and free across each category
![image](https://user-images.githubusercontent.com/70737240/233856412-9a7a4919-96c9-4d38-8fca-a8ac9164366f.png)
---
7. Exploring correlations
![image](https://user-images.githubusercontent.com/70737240/233856474-14b6dc0b-88a7-4a00-995a-e81fd9225472.png)
---
Conclusion - we can see that reviews and number of installs have high correlation
---
8. Sentiment Analysis - User reviews across each category
![image](https://user-images.githubusercontent.com/70737240/233856504-b1cdf1e1-14dc-4375-aa23-90ef3d5e092a.png)
---
Conclusion - AUTO_AND_VEHICLES and HEALTH_AND_FITNESS receive the most positive reviews. Whereas GAMES receive the most negative reviews
---
9. Visualising sentiment polarity distribution across paid and free apps
![image](https://user-images.githubusercontent.com/70737240/233856550-931190ab-6984-40ff-97bf-d81f983f1e64.png)
---
Conclusion - we can see that the free apps receive more harsh reviews as compared to paid apps
---
note : Some of these visualisations are present in the notebook but others did not show. But if you happen to run the notebook they should how up just fine.
