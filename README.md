# 2023_ZT_TWBiobank
9/2023 ~ 6/2024 專題 with topic : Taiwan Biobank 

Anything related to this 專題 will be posted here. For more important documents that are confidential will be locked with a password.
Please ask me for the password if you need to access the file.

Note: The confidentiality and any other issues regarding the dataset will be discussed thoroughly with the Professor and the real dataset, whole or in parts, will never be posted online.

## ---11/29---
We talked about zhuanti vs data viz:
1. For Zhuanti
   - Fancier data introduction (similar to one from the webiste)
   - More complicated graphs
   - Make appearance look better
2. For data viz
   - Just show simpler graphs
   - Simple plot and interaction
   - Data introduction (not necessary)
3. For both
   - Plot more graph

The point is, even though the idea is the same for zhuanti and data viz make sure they don't look the same.

Another thing is to answer the questions that the teachers have from the midterm:
1. Literature review
   - Biobank pattern analysis : https://diglib.eg.org/handle/10.2312/eurova20171118
   - Visual analytics for biology (vis tool) : https://ehjournal.biomedcentral.com/articles/10.1186/1476-069X-8-61
   - Others: This paper is a review paper so it talk about a lot of health and visualization thing and you can see the references the use: https://onlinelibrary.wiley.com/doi/full/10.1111/cgf.13891

2. Recommendation to talk to domain expert:
    - Instead of finding a domain expert what we can do is find papers that confirm our findings. For example, this paper confirm that Kidney stone disease correlates to obesity attributes like BMI, WHR, etc. https://pubmed.ncbi.nlm.nih.gov/34714367/#:~:text=BMI%2C%20WC%2C%20WHtR%2C%20WHR%2C%20AVI%2C%20and%20BRI,of%20KSD%20in%20clinical%20practice.

In addition, that paper is for the biobank (but to find paper that confirm we don't have to use biobank paper). 

You can just write something like "Our result of bla bla bla is confirmed by other papers' findings [references]"

About future work (next midterm and final)
Find patterns in diseases:
1. Correlation
2. XGBoost or any boosting algorithm to do prediction, I think Professor prefer Adaboost. Either one is fine and its the easiest way imo
3. Or based on the Profesor opinion, maybe also try decision tree.

Just a reminder:
Make sure your ppt have :
1. Answers for the previous questions the profesors asked during presentation
2. Some literature (just talk about it fast)

## ---10/13---
The logic flow of this project is:
1. We have the Taiwan Biobank Dataset
2. Due to the different type of information in the dataset, users might find it hard to find any patterns from the dataset
3. We create a tool that will help make it easier for users to find pattern
(It is not impossible to find patterns from the dataset without using our tool, the aim to create a tool is just to make it easier and save more time)

Big goal (the whole project): Create a tool to help find hidden patterns from the dataset

Small goals:
1. Using simple methods, some examples:
   - Find disease distribution (which disease is more commonly found in Taiwan?)
   - Find gender distribution in disease (are there more male or female people with Diabetes?)
   - Find disease distribution in different location (are gout more likely to be found in the northern part of Taiwan?)
2. Using more complicated methods,
   we acknowledge that there are limitation when only using simple methods. For more in-depth questions (Example: What eating habits have a high influence on people getting Hypertension?) it is necessary for us to have a more compicated methods, because of that in the near future, when we're done with the preliminary studies the next steep will me to use a more complex methods like:
   - Correlation value
   - Dimension reduction
   - Machine learning/deep learning

## ---9/13---

For the time being, it is recommend you to learn more about:
  1) Data preprocessing (pandas)
  2) Data visualization (basic D3)

The plan for now is to recreate the webtool page 01 that I have written here (http://140.122.185.208/~lienathania/SinicaProj/Page01_DiseaseDistribution_ver4/)

Breakdown of the page01 webtool

First, filter the dataset we're only using BASELINE data (people 1st time checking) and we're not going to use any FOLLOW UP data
  - Bar chart (https://d3-graph-gallery.com/barplot.html)

      **We don't count the family members in this bar so only count _SELF**
    
      - Sort by highest to lowest
      - Sort by high to low and also by groups
      - Normalized the bars
      - Log scale the bar
      - Add interaction (tooltip, and console.log the name of the disease when clicked => it is important we know how to get the name/id of the disease chosen since we need that to draw the rest of the graphs)
  - Map (https://d3-graph-gallery.com/choropleth.html)
      - Draw Taiwan map from json file
      - Colored based on the number of people with the disease
      - Colored based on the normalize value of it
      - Add interaction (tooltip)
  - Pie chart (https://d3-graph-gallery.com/pie.html)
      - Show the distribution of people with the disease in the family
      - Show the distribution of gender from people with the disease
      - Add interaction (tooltip)
  - Bar chart
      - Showing 2 bars side by side for age distribution
      - Showing 2 bars side by side for family distribution
      - Add interaction (tooltip)
  
You don't have to make exactly what I did. If when you explore the dataset, you feel like you want to try something else also no problem.

Due to the confidentiality regarding this dataset, I will only post **toy dataset** here (the columns will be real but the values will be randomized). If there are any changes in the rules or more flexibility I will let you know. 


---
If there is anything you need from me please let me know, I'll be happy to help

Sincerely,

Tia
