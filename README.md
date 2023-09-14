# 2023_ZT_TWBiobank
9/2023 ~ 6/2024 專題 with topic : Taiwan Biobank 

Anything related to this 專題 will be posted here. For more important documents that are confidential will be locked with a password.
Please ask me for the password if you need to access the file.

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
