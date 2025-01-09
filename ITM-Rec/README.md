## Data Description

ITM-Rec data sets including student and group preferences on the topics of final projects in data base and data science classes, and it was collected from student questionnaires at the ITM department, Illinois Institute of Technology, USA. It can be utilized for the purpose of developping and exmining different educational recommender systems (RS), e.g., context-aware RS, multi-criteria RS, group RS, and RS with integrated information, such as multi-criteria based context-aware RS, context-aware based group RS, and so forth.

For more information, you can refer to the two publications below:
 - Yong Zheng. "[ITM-Rec: An Open Data Set for Educational Recommender Systems](https://github.com/irecsys/RecData/blob/main/ITM-Rec/ITM-Rec_LAK23.pdf)". Companion Proceedings of the 13th International Conference on Learning Analytics & Knowledge (LAK), Arlington, TX, USA, March 13-17, 2023
 - Yong Zheng. "Personality-Aware Decision Making In Educational Learning", Proceedings of the 23rd ACM Conference on Intelligent User Interfaces (ACM IUI), Tokyo, Japan, March 7-11, 2018
 
Notes: Students' personality traits were not disclosed in this data set, due to privacy concerns.

## Citations

If you used this data for the purpose of research, please cite the following publications:
 - Yong Zheng. "[ITM-Rec: An Open Data Set for Educational Recommender Systems](https://github.com/irecsys/RecData/blob/main/ITM-Rec/ITM-Rec_LAK23.pdf)". Companion Proceedings of the 13th International Conference on Learning Analytics & Knowledge (LAK), Arlington, TX, USA, March 13-17, 2023
 
```
@inproceedings{zheng2023itm,
  title={ITM-Rec: An open data set for educational recommender systems},
  author={Zheng, Yong},
  booktitle={Companion Proceedings of the 13th International Conference on Learning Analytics & Knowledge (LAK)},
  year={2023}
}
```

## File Descriptions

 - users.csv   
   columns: UserID, Gender, Age, Married   
   description: Meta data about students
 - items.csv   
   columns: Item, Title, URL, Descriptions  
   description: Meta data about the topics of projects
 - ratings.csv   
   columns: UserID, Item, Rating, App, Data, Ease, Class, Semester, Lockdown  
   description: Students' individual ratings on items, including the overall rating (i.e., the column 'Rating'), and multi-criteria ratings (i.e., ratings in 'App', 'Data', 'Ease'), as well as three contextual variables, e.g., class, semester, lockdown
 - group.csv   
   columns: GroupID, UserID  
   description: the compositions of groups
 - group_size.csv  
   columns: GroupID, Size   
   description: the number of students in each group
 - group_ratings.csv   
   columns: GroupID, Item, Rating, App, Data, Ease, Class, Semester, Lockdown  
   description: Ratings on items given by groups, rather than individuals

## Data Statistics
	
	Ratings by individual students:
	# of users: 476
	# of items: 70
	# of ratings by individual users: 5230
	distribution of rating amounts by users: {mean: 11.52, min: 3, max: 51, std: 7.06}
	distribution of rating stars (Rating): {1: 724, 2: 1050, 3: 555, 4: 1348, 5: 1553}
	distribution of rating stars (App): {1: 514, 2: 862, 3: 1062, 4: 1492, 5: 1300}
	distribution of rating stars (Data): {1: 421, 2: 872, 3: 1284, 4: 1549, 5: 1102}
	distribution of rating stars (Ease): {1: 474, 2: 900, 3: 1713, 4: 1511, 5: 632}
	
	Ratings by student groups:
	# of groups: 143
	# of items: 70
	# of ratings by groups: 1117
	group size: {2: 88, 3: 42, 4: 9, 5: 4}
	distribution of rating amounts by groups: {mean: 7.81, min: 5, max: 22, std: 2.47}
	distribution of rating stars (Rating): {1: 115, 2: 306, 3: 172, 4: 2244, 5: 280}
	distribution of rating stars (App): {1: 87, 2: 229, 3: 281, 4: 292, 5: 228}
	distribution of rating stars (Data): {1: 63, 2: 227, 3: 309, 4: 333, 5: 185}
	distribution of rating stars (Ease): {1: 78, 2: 205, 3: 344, 4: 355, 5: 135}
