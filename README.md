# Shopify-Data-Analysis

Objective : In this project, Shopify app store data from April 1,2013 to September 9, 2019 was used to identify patterns within app rating review and create clusters based on apps description using word embedding

Motivation : The project was motivated with a personal agenda. With the world moving online, my brother in law wanted to move his shop online and asked me if there was an option. I had heard about shopify but did not know how it worked.  App reviews and App Description were main focus of the analysis.

Data : There were 6 readily available dataset. Out of 6, 4 were used within this project.
1. apps.csv - The file contains the information for different apps, developer details, app rating, review count and description
2. apps_categories.csv - The files contains information for the categories of the app. There were 12 different categories identified
3. categories.csv - This is the lookup file for the category code from the above
4. reviews.csv - This file contains the review given for each app along within the rating 

Analysis and Results : Teh following analysis was performed:
1. Created a Pie Chart using plotly to show the category distribution. Among the 12 categories, 28.6% was classified as Store design, 17.8% as Sales and conversion  and 14.8% as Marketing. The average review count disctribution confirmed that the most used categories have been reviewed the highest. 
2. Stacked chart was created to show the number of apps created by each developer along with average rating. It was discovered that some of the apps were never used at all.
3. The ratings for the review left on the app was cleaned to to identify the commonly occuring word combination to describe the lowest rated reviews. It was discovered that the bad customer servive and faulty application were the main cause of the lowest rated app.
4. Finally, kmeans clustering was performed on the app description to identify app segmentation. word2vec algorithm was used to identify the relationship between words and embed them in lower dimensional vectory space. Using this, kmeans clustering was performed with the optimum cluster size = 3 and silhouette score of 0.336. Finally, word embedding visualization was created using T-SNE to display the similiar objects.

