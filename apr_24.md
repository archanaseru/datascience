



```
Data science and Aritificial Intelligence:

------------------------------------------
	1. statical essentials for DS
	2. Linear algebra -- for predictions.
	3. Machine Learning
	4. Neural Networks
	5. Deep Learning
	6. NLP
	7. Generative AI  


Data science and AI
 ---------------------

 Data Analyst vs Data science ?
 -----------------------------
----> VISUALIZATIONS (python, tableau, powerbi, Qlikview)
---> statistical analysis
	---> predictions
	--> forecasting.

   statistical predictive modeling -->
	problem --> Complex patterns can not be unstertood
			by statistical models.

data scientist -->
   all works of data analyst with advanced techniques
	ex:
		1. Machine learning
		2. NN
		3. Deep Learning
		4. NLP (Natural language processing)
			--> pre processing of the text
			--> analysis on text data.
				--> ex: sentiment analysis (customer reviews)

*----------------------------------------------
Data science  Vs Artificial Intelligence ?

    Data scientist  Vs  AI developer(Engineer)   ?
   --------------------------------------

      Common skill set for both:
		1. ML
		2. NN and DL
		3. NLP
		etc.

#---------------------------------------------------------------------------

data scientist ---> building models

	process of bulding model:
	--------------------------
		1. preprocess of data
			(data cleansing)
			(data transformations)
		2. data preperation
			ex: X-train, X-test, Y-train, Y-test
		3. model selection
		4. Train model (train the predictive model)
			--> who trainer ? --- you (data scientist)
			--> who is learning ? -- model (math predictive equation)
			--> what model learns ?
				--> relationships between features(input variables) and labels(target variables)
				---> technically , the knowledge of model (relationships)  is called model fit.

		model vs "model fit"
			model --> math predictive equation
			model fit --> is knowledge of model

                  5. model evaluation (accuracy testing).
#-------------------
 before training --> model has random knowledge(bad)--> bad model fit

 after training ---> model has good knowledge ---> best model fit.

    ex:   Y = X . W

		X --> feature matrix
		Y --> label matrix

		W --> Weight Matrix ---> model fit


once model is build for a prediction,

what data scientist ,
	he applies   trained model (fit) on new data,
	based on output of the model , He does predictions.

after training :
	Y = X. W
	--> X --> featuress ---> age, wgt, height-->100 patients
	--> Y --> labels --> cholestral  ---> 100
	    W --->  (4,1 )   ---> rows , 1 column


		ex:  [ [ 0.5],           --> bias
			[2]		 --> slope of first variable   (age)
			[3]		---> slope of 2nd variable	(wgt)
			[1.5] ] (4, 1)   ---> slope of 3rd variable	(hgt)


new data of new patients>


age,wgt,hgt
30,60,5.5
40,80,5.6
35,54,5.8

task : based on new patients age, wgt, hgt predict cholestral


PX = [[ 1, 30, 60, 5.5],
      [ 1, 40, 80, 5.6],
      [ 1, 35, 54, 5.8]]

PY = PX.dot(W)
    3X4   4X1
       3X1

    [[30],
     [45]
     [50]]

doctor's bench mark  , less than 40 --> no risk
	    greater than or equals to 40 --> risk.

    [[30],     ---> NoRisk
     [45]      ----> Risk
     [50]]     ---> risk




( ds --> by applying trained model fit for new data, he does predictions manually)

 ---------------------------------------------------------------------------
AI engineer = ML(NN+DL) + MLOps + LLMOps(gen ai)

    ---> trained model and model fit --> has to deployed into production application.

 once trained model is deployed into application,
	The application will become as AI application, which can behave like human about specific task.


#---------------------------------------------

