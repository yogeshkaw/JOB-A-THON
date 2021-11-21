### JOB-A-THON
### Approach

## Pre-Processing 

* Converted qualitative variable into integers value (ie Gender, Education_Level)
* ##New Features (Information extraction):- 
   * emp_tenure:-  Calculated Age of Employe or Employe tenure (number of days in the company)
   * TBV_difference:- This feature represent difference of Total Business Value as compare to last month.
   * number_of_promotion:- This represent number of times employe get promoted

* With the help of feature LastWorkingDate, I calculated whether an employe got churned, and we stored that information in Target column.
* If an employee is churned, Then I have assumed that employee is churned before 9 month (ie if employee is churned on 1/9/2021 then I assumed that he is churned on 1/1/2021). I have assumed this because when an employe is about leave an organisation we can observe change in the behaviour of employe even before notice period. This can also a considered as a hyper-parameter.
* I dropped few features like city,  LastWorkingDate, Dateofjoining etc
* After that I separated test data from training data ( As Its a panel data I took latest date and separated train and test data)
* Finally I used GradientBoosting algorithm for prediction.  
