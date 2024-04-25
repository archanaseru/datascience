
module 1: stat and linear algebra. 
     
  statistics:
  -----------
       what is statistics ?
	--> is sub descipline of Mathematics .
		--> used for scientific analysis of the data 
			(includes understanding patterns, moments , 
			 predictions, forecasting  ....)
      
     " Statistics is a scientific approach to analyse the data "

	what is scientific approach ?????????????
  	--> Any conclusion should be made with some mathemetical measurement proof .


	what is dependecy between  temperature and "ice cream" sales?

		correlation(tempr, ice_sales) -->r = 0.98		
		  r >0 --> positive correlation between  tmpr and ice. 

		  interpretation -->
			as tmpr increases, sales of icecream increases.
			as tmpr decreases, sales of icecream decreases. 


		correlation(tempr, swetter_sales)
			---> r= -0.92
		r < 0 --> negative correlation bw   tmpr and swetter

		
		correlation(tempr, ai_training_sales)


			tmpr	ai_training_sales
			--------------------------
			10		5L
			15		5.5
			25		4.9
			30		5L
			--------------------------

		corr(tmpr, ai)
			-->r = 0.003

		   ---> r ~= 0 ---> no dependency between  tmpr, ai


    which prediction are possible ?

	1. predict ice_creame sales  , if tmpr is 35. --> possible --> dependency

	2. predict swetter sales value, if tmpr is 40 --> possible --> dependency

	3. predict ai_sales value, if tmpr is 39 --> no possible --> no dependency


#---------------------------------------------

 two types of statistical analysis ----->

     1. Descriptive statistics
     2. Inferential statistics


1. Descrptive stat -->
	Analysis over population data. 

2. Inferential stat -->
	Analysis over sample data. 



scenario 1;
   you are Hr head  of IBM organization. 

   question:
	what is avg salary of ibm software engineers ?
		----> population


scenario 2:
      you wanted to start a obesity centre at hyderabad. 
	
    question:
	what is avg weight of hyderbad females aged between 20 to 40. ?
		---> sample

		--> avg(w) of f(20-40) is 45kg

descriptive :
	apply analysis over population data, 
		and conclusion on entire population. 

   example
	what is avg salary of ibm software engineers ?
		----> population

Inferential :
	apply analysis over sample data,
		and conclusion on entire population

how much sample size to be collected ?


     ---> based CI test. (Confidence Interval)

#------------------------------------------------------------------------
5 lakhs

	1. size		avg		ci
	-------------------------------------
	   200		56		0.9
	   500		50		0.7  --> diff
	   1000		52		0.1  ---> diff
	   1500		48		0.05  ---> diff
	   2000		47		0.03 ---> diff
	   2100		47.02		0.02999 --> neglectable diff (you can stop
						      collecting new data)
	--------------------------------------------
	   
conclusion -->
	Avg weight of females of aged 20 to 40   is  "47" with CI 0.03
	   
	   
#------------------------------------------

two types of data analysis in statistics ---> 
	1 . Uni Variate analysis.
	2 . Multi variate analysis. 


1. Univariate ---> 
	analysis over single variable.

2. multivarite --> 
	analysis over multiple variables. 



	sachin, gangooly
you have data of 100 matches runs of sachin and gangooly. 
Given data:
	cricket_runs.txt
	----------------
	sachin	gangooly
	-----------------
	70	90
	90	86
	90	0
	100	96
	:
	:
	0	70
	-----------------------
question 1:
   who is best player ? based on runs

	--> statistical instrument is "mean"

	mean(sachin) --> 90--> most of sachin runs are near to 90
	mean(gangooly) --> 70 --> most of sachin runs are near to 70

    what is stat instrument ? ---> mean
   mean applied seperately on sachin, seperately on gangooly. 

	at a time stat instrument is applied on "single" variable.

   --> above question comes under "Univariate Analysis". 

 




question 2:
   what is dependency between sachin and gangooly. 

     to solve this problem, what is stat instrument ?
	---> correlation. 

	correlation(sachin, gangooly) --> r =  -0.79

	   ---> negative correlation

	stat instrument at a time applied on two variables. 
	--> above comes under "Multi variate analysis". 

Question 3:
	if sachin hits 30 runs, 
		predict  gangooly runs?

	step1.
		there should be correlation(dependency) between variables. 
		  correlation(sachin, gang)
			--> r= -0.79
	step2 . prediction. 
		-> stat instrument
		Regression
			y = a + bx
		 x --> sachin
		b --> slope of sachin
		a --> intercept
		y --> predicted score of gangooly

	in both steps, 
		stat instruments at a time applied on 2 variables. 

    --> above question comes under multi variate analysis. 

#------------------------------------

Univariate Analysis ---> 
-------------------------
   1. MCT (measure of Central tendency)
	--> Mean
		--> Arithmetic mean
		--> Geometric mean
		--> Harmonic mean
	--> Mode
	--> Median
		--> Quartile 1
		--> Quartile 2
		--> Quartile 3
   2. Dispersions:
	--> Range
	--> variance
	--> Standard deviation. 

Multivariate Analysis:
-----------------------
	--> Covariance
	--> Correlation
	--> Regression
		---> Linear Regression
		---> Non Linear Regression
		--> Logistic Regression
	---> Forecasting

#---------------------------------------------------------------
	
MCT --> measure of Central tendency. 

   (mmm) --> mean, mode, median
purpse of MCT --> 
   to understand about a variable performance with a single value. 


aggregation functions --> 
	sum() , count(), max(), min(), avg()...

sum --> rejected from mct list
count --> --> rejected from mct list
max --> rejected from mct list
min --> rejected from mct list

avg --> accepted as  mct


#---------------------
  sum(sachin) ---> 10000 --> independently sum() not able to explain performancce.
	he gave 10000 runs 

   max(gangooly) --> 170 
   min(sachin) ---> 0

independently above aggregated functions, 
	sum(), count(), max(), min() can not explain variable performance. 
	thats why rejected from MCT list. 


---------
 mean(sachin) ---> 80
    interpretation --> most of sachin scores are close to 80
	--> it explains performance. 
my students data:
  mode(gender) ---> 'male'
	--> most of students are "males"
	--> explains performance

  median(sachin) --->     60 
	in 50% of matches sachin gave above 60. 
	in 50% of matches sachin gave below 60

  ex: sachin played 1000 matches. 
	--> in 500 matches, he gave above 60
	--> in 500 matches , he gave below 60 
     --> explains performance


*-----------------------------------

i have 700 students for AI
   300 students got job as AI dev
     mode(300_ai_gender)--> "male"

--> interpretation --> most of successful students are "males"
   --> explains performance 

all above mean, mode, median are explaining performance of a variable. 

those are part of "MCT"
******************************************************

Mean--> average  --> most of values are close to mean
Mode --> highly repeated. --> most probably the next event would be "mode"
Median --> central value.--> 50% of data are above to median
			     50% of data is below to median

#---------------------------------------------




     





