
 <div align='center' > 
  <h2> International Conference on Database Systems for Advanced Applications </h2>
 </div>

 <div align='center' style = "vertical-align:middle"> 
  <h2> <a href="http://www.tjudb.cn/dasfaa2023/"> DASFAA 2023 </a><a href="http://www.tjudb.cn/dasfaa2023/">(http://www.tjudb.cn/dasfaa2023/)</a> </h2>
 </div>

## Workshop:
**Bundle-based Recommendation Systems**


## Abstract:

Bundle is a collection of items with similar styles or complementary functions, such as music playlists and fashion outfits. Bundle recommendation aims to accurately predict the probabilities of user interactions with bundles. Meal recommendation is an application of bundle recommendation in food scenarios. Its task is to provide courses(items) that are enjoyed as a meal(bundle) for a user. However, research on meal recommendation has made little progress compared to other well-studied domains such as product bundle, music playlist, travel package, etc. It is highlighted that the major obstacle is lacking public datasets specializing in meals for research community. 

This workshop issues a suit of MealRec datasets with different interaction densities from a public recipe data via a category-constrained meal construction method. The workshop will bring together researchers and professionals from academia and industry from around the world for showcasing, discussing, and reviewing the whole spectrum of technological opportunities, challenges, solutions, and emerging applications in efficient but robust meal recommendation using state-of-the-art techniques. Through calling participants to submit their meal recommendation results on our breadboards, their build bundle recommendation models can be evaluated to identify promising techniques based on this public meal dataset. 

**Topics of particular interest include, but are not limited to:**

* GNN and Transformer exploiting on bundle recommendation
* Multimodal learning on bundle recommendation
* Model distillation and designing for bundle recommendation
* Cold start problem in bundle recommendation 
* User preference learning
* Exposure bias problem in bundle recommendation
* Explanation of bundle recommendation model

## Organizing Team

| ![avatar](./picture/1.png) |![avatar](./picture/2.png) |
| :-: | :-:|
|  Prof. Lin Li, Wuhan University of Technology, China |Dr. Jianquan Liu, NEC Corporation, Japan |


## Important Dates

* Training data ready: November 15 2022
* Test evaluation starts: December 15, 2022
* Paper submission due: TBD
* Notification of Acceptance: TBD
* Camera-Ready Papers Due: TBD
* Workshop date: April 17, 2023


## Publication

DASFAA (Database Systems for Advanced Applications) is an annual international database conference, typically located in the Asia Pacific region, aimed at showcasing the state-of-the-art and the broad range of activities in database-related research and development. It provides a forum for technical presentations and discussions among database researchers, developers and users from academia, business and industry.

The 28th DASFAA conference will be held from 17-20 April 2023 in Tianjin, China.

The papers accepted by DASFAA 2023 workshop will be published in a combined volume of Lecture Notes in Computer Science series published by Springer, and indexed by both LNCS and DBLP.

## Data Description

The suit of MealRec datasets we released contains two datasets, MealRec-77 with a user-meal interaction density of 0.77% and MealRec-17 with a user-meal interaction density of 0.17%.  

Each dataset contains 4 .txt files and 2 .csv files.  The .txt files only contain the ID field to record the relationship between entities, and the .csv files contain rich description information of recipes and user reviews on recipes. The detailed description and fields   of these files are as follows: 

- user_recipe.txt : the interaction information between users and recipes;
  - user_id : user  identifier
  - recipe_id : recipe  identifier
- recipe_category.txt : the correspondence information between recipes and categories;
  - recipe_id : recipe  identifier
  - category_id : category  identifier
- meal_recipe.txt : the affiliation information between meals and recipes;
  - meal_id : meal  identifier
  - recipe_id : recipe  identifier
- user_meal.txt : the interaction information between users and meals. This file is divided into training set, verification machine and test set according to the ratio of 8:1:1. The training set and verification set have been given, and the test set will be given later;
  - user_id : user  identifier
  - meal_id : meal  identifier
- recipe.csv :  rich descriptive information about recipes;
  - recipe_id : recipe  identifier
  - recipe_name : the name of the recipe 
  - aver_rate : average user ratings(five-point scale) 
  - image_url : the url of the recipe image
  - ingredients : ingredients included in the recipe 
  - cooking_directions : food making process
  - nutrition : nutritional content information of this food
  - review_num : total number of the recipe’s reviews
  - reviews : all reviews of the recipe
  - tags : several tags selected by the creator represent features of the recipe
- user_recipe.csv : details of the user's interaction with the recipe.
  - user_id : user identifier 
  - recipe_id : recipe identifier 
  - rating : user ratings for the recipe(five-point scale) 
  - dateLastModified : the time the user review was last modified 