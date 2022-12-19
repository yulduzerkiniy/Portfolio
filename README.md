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

