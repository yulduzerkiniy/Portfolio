<div align="left">
  
  
# Data Science Portfolio
### Hi there! I'm Yulduz! I tried to share my most different Data Science projects.
#### In this page you will see the explanation and some conclusions and results.
#### At the end of each project there's a link to source code
  
  
<!-- Table of Contents -->
# :notebook_with_decorative_cover: Table of Contents

- [Project 1](#star2-about-the-project-1)
  * [Data 1](#camera-data-1)
  * [ML](#dart-ml)
  * [Source Code](#scroll-source-code)
- [Project 2](#star2-about-the-project-2)
  * [Data 2](#camera-data-2)
  * [Exploratory Data Analysis](#dart-exploratory-data-analysis)
  * [Source Code 2](#scroll-source-code-2)
- [Project 3](#star3-about-the-project-3)
  * [Data 1](#camera-data-3)
  * [ML](#dart-ml)
  * [Source Code](#scroll-source-code)
- [Contributing](#wave-contributing)
  * [Code of Conduct](#scroll-code-of-conduct)
- [Contact](#handshake-contact)

  

<!-- About the Project 1-->
## :star2: About the Project 1
### School students final grade prediction
#### This data approach student achievement in secondary education of two Portuguese schools. The data attributes include student grades, demographic, social and school related features) and it was collected by using school reports and questionnaires. Two datasets are provided regarding the performance in two distinct subjects: Mathematics (mat) and Portuguese language (por). 
#### The main purpose is to predict sutends' final grade based on their family backgound, school, their previous grades and other attributes. The technique used in this project is CatBoost Regressor, which managed to show quite good results.
#### Here's the initial data:
  <!-- Data 1 -->
### :camera: Data 1

<div align="center">

  <img src="images/students_df.png" alt="dataset" width="1000" height="auto" />
  
<div align="left">
  
 #### The initial thought was that the final grade may depend on the address attribute (urban/rural areas) and also may depend on the sex of a student. But apparently, they was not the most important attributes for the final grade: both of them have similar distributions:
  
  <div align="center">

  <img src="images/G3_sex.png" alt="Final_grade_sex" width="500" height="auto" /><img src="images/G3_address.png" alt="Final_grade_address" width="500" height="auto" />
    
<div align="left">
  
 #### Obviously, the final grade strongly depends on the previous failures of a student. The higher the number of failures, the less the final grade:
    
 <div align="center">

   <img src="images/G3_Failures.png" alt="final_grade_failures" width="600" height="auto" />

 
<div align="left">
  
### ML
  <!-- ML -->
### :dart: ML
#### The model used in prediction is CatBoost regressor, which is quite good at handling categorical features. The model showes quite good results:
  
 <div align="center">

   <img src="images/metrics.png" alt="metrics" width="400" height="auto" />
   
<div align="left">
  
#### Also real and predicted target values:
  
<div align="center">

   <img src="images/y_test_y_redicted.png" alt="y_pred" width="400" height="auto" />
 
  
<div align="left">
  
<!-- Source Code -->
### :scroll: Source Code
  
  https://github.com/yulduzerkiniy/Portfolio/tree/main/students_grade
  
  
  

<!-- About the Project 2-->
## :star2: About the Project 2
#### A common question for those new and familiar to computer science and software engineering is what is the most best and/or most popular programming language. It is very difficult to give a definitive answer, as there are a seemingly indefinite number of metrics that can define the 'best' or 'most popular' programming language. One such metric that can be used to define a 'popular' programming language is the number of projects and files that are made using that programming language. As GitHub is the most popular public collaboration and file-sharing platform, analyzing the languages that are used for repositories, PRs, and issues on GitHub and be a good indicator for the popularity of a language.


  <!-- Data 2 -->
### :camera: Data 2
  
#### This dataset contains statistics about the programming languages used for repositories, PRs, and issues on GitHub. The data is from 2011 to 2021. This data was queried and aggregated from BigQuery's public github_repos and githubarchive datasets. Only data for public GitHub repositories, and their corresponding PRs/issues, have their data available publicly. Thus, this dataset is only based on public repositories, which may not be fully representative of all repositories on GitHub.

<div align="center">

  <img src="images/repositories_df.png" alt="dataset" width="200" height="auto" /><img src="images/issues_df.png" alt="dataset" width="270" height="auto" /><img src="images/pl_df.png" alt="dataset" width="250" height="auto" />
  
<div align="left">
  
  
### Exploratory Data Analysis
  <!-- Exploratory Data Analysis -->
### :dart: Exploratory Data Analysis
#### Obviously over the dacade JavaScript is definitely the most 'popular' language among others:
  
 <div align="center">

   <img src="images/repos_numbers.png" alt="metrics" width="600" height="auto" />
   
<div align="left">
  
#### The same idea gives this pie chart:
  
<div align="center">

   <img src="images/repos_precentage.png" alt="metrics" width="400" height="auto" />
   
<div align="left">
  
#### Quite intuitive to think that big number of repositories leads to more issues:
  
<div align="center">

   <img src="images/issues_numbers.png" alt="metrics" width="600" height="auto" />
   
<div align="left">
  
#### To confirm the thought:
  
<div align="center">

   <img src="images/issue_per_repos.png" alt="metrics" width="600" height="auto" />
   
<div align="left">
  
#### However! Can we simply make a such a conclusion? According to the trends for each year Javascript lost its popularities starting in 2017. And after several years it completely missed its position losing to Python:
  
<div align="center">

   <img src="images/issues_per_year.png" alt="metrics" width="600" height="auto" />
   
<div align="left">
  
#### Let's try to demostrante it by means of pull requests percentage in 2012 and 2021:
  
<div align="center">

   <img src="images/pl_2012_2021.png" alt="metrics" width="800" height="auto" />
   
<div align="left">
  
#### Some fency 3D distribution graph for some popular languages for each year:
  
<div align="center">

   <img src="images/languages_3d.png" alt="y_pred" width="600" height="auto" />
 
  
<div align="left">
  
<!-- Source Code 2 -->
### :scroll: Source Code 2
  
  https://github.com/yulduzerkiniy/Portfolio/tree/main/programming_languages_Data_Visualization
  
  

<!-- About the Project 3-->
## :star2: About the Project 3
### eCommerce store events data analysis
#### This file contains behavior data for Nov 2019 from a large electronics commerce online store.
Each row in the file represents an event. All events are related to products and users. Each event is like many-to-many relation between products and users.
Data collected by Open CDP project.
#### The main purpose is to group customers into several categories. Several approaches have been used, like RFM which is widely used in marketing and k-means machine learning approach.
#### Here's the initial data:
  <!-- Data 3 -->
### :camera: Data 3

<div align="center">

  <img src="images/students_df.png" alt="dataset" width="1000" height="auto" />
  
<div align="left">
  
 #### Quite obvious that users usually view a lot before adding something to cart. After that they can actually purchase desired items:
  
  <div align="center">

  <img src="images/G3_sex.png" alt="Final_grade_sex" width="500" height="auto" /><img src="images/G3_address.png" alt="Final_grade_address" width="500" height="auto" />
    
<div align="left">
  
 ### RFM
 #### RFM is a method used for analyzing customer value. It is commonly used in database marketing and direct marketing and has received particular attention in retail and professional services industries.

 #### RFM stands for the three dimensions:
    Recency – How recently did the customer purchase?
    Frequency – How often do they purchase?
    Monetary Value – How much do they spend?

#### source: https://en.wikipedia.org/wiki/RFM_(market_research)

#### In this method I'm trying to divide customers to categories, highlight the loyal and regular customers; identify customers who were loyal before in order to 'remind' about some new sales/services
  
###  Segmentation using k-means

#### Using some manimulations like MinMaxScaler, PCA to help clusterization algorith, and kMeans to clusterize, we got simple customers classification to "Loyal customers" and not so much.
  
#### Quite obvious that we can split customers to groups. In this case I decided to divide them into 2 groups. Group1 are people whose last purchase was quite a lot time ago, spent less money and not many purchases. Whilst, for Gruop0 is quite opposite. Last purchase mean is 9 days ago, spent in average $700, mean number of purchase is 2. Also, quantiles looks better
  
### RFM Segmentation
  #### https://www.optimove.com/resources/learning-center/rfm-segmentation
  
  #### The first step in building an RFM model is to assign Recency, Frequency and Monetary values to each customer.
  #### The second step is to divide the customer list into tiered groups for each of the three dimensions (R, F and M). Unless using specialized software, it’s recommended to divide the customers into four tiers for each dimension, such that each customer will be assigned to one tier in each dimension. This results in 64 distinct customer segments (4x4x4), into which customers will be segmented.
  #### The simplest way to create customers segments from RFM Model is to use Quartiles. We assign a score from 1 to 4 to Recency, Frequency and Monetary. Four is the best/highest value, and one is the lowest/worst value. A final RFM score is calculated simply by combining individual RFM score numbers.
  
  <div align="center">

   <img src="images/languages_3d.png" alt="y_pred" width="600" height="auto" />
 
  
<div align="left">
  
 <div align="left">
  #### The third step is to select groups of customers to whom specific types of communications will be sent, based on the RFM segments in which they appear.
   
   
#### It is helpful to assign names to segments of interest:
   **Best Customers** – This group consists of those customers who are found in R-Tier-1, F-Tier-1 and M-Tier-1, meaning that they transacted recently, do so often and spend more than other customers. A shortened notation for this segment is 1-1-1; we’ll use this notation going forward.
   
   **High-spending New Customers** – This group consists of those customers in 1-4-1 and 1-4-2. These are customers who transacted only once, but very recently and they spent a lot.
   
   **Lowest-Spending Active Loyal Customers** – This group consists of those customers in segments 1-1-3 and 1-1-4 (they transacted recently and do so often, but spend the least).
   
   **Churned Best Customers** – This segment consists of those customers in groups 4-1-1, 4-1-2, 4-2-1 and 4-2-2 (they transacted frequently and spent a lot, but it’s been a long time since they’ve transacted).
  
 <div align="center">

   <img src="images/G3_Failures.png" alt="final_grade_failures" width="600" height="auto" />

 
<div align="left">
  
### Wider RFM segmentation
  <!-- ML -->
### :dart: ML
#### Now that we've identified our customer categories, we can decide how to approach or deal with each customer.
  
#### Link to the article:
https://documentation.bloomreach.com/engagement/docs/rfm-segmentation
  
 <div align="center">

   <img src="images/metrics.png" alt="metrics" width="400" height="auto" />
   
<div align="left">
  
#### Also real and predicted target values:
  
<div align="center">

   <img src="images/y_test_y_redicted.png" alt="y_pred" width="400" height="auto" />
 
  
<div align="left">
  
<!-- Source Code -->
### :scroll: Source Code
  
  https://github.com/yulduzerkiniy/Portfolio/tree/main/students_grade
  
  
  
  
  
  
  

<!-- Contributing -->
## :wave: Contributing

<a href="https://github.com/yulduzerkiniy">
  <img src="https://avatars.githubusercontent.com/u/94949957?s=400&u=f210a81d44eae02daaa30be637a8cb42afb692c4&v=4" alt="y_pred" width="50" height="auto"/>
</a>

 
Contributions are always welcome!

See `contributing.md` for ways to get started.



<!-- Contact -->
## :handshake: Contact

Your Name - [@linkedin](linkedin.com/in/yulduz-erkiniy-228354248) - yerkiniy@gmail.com

Project Link: https://github.com/yulduzerkiniy/Portfolio

