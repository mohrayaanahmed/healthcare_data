# healthcare_data
# **Predictive models on healthcare data**
*Using Machine Learning algorithms to build two predictive models in achieving two distinct objectives*

**Objective I:**
The first objective is to build a predictive model that would predict the type of operation a patient is likely to have based on the type of hip fractures suffered. There is two images attached describing the different types of hip fractures.

**Objective II:**
The second objective is to establish relationships between different diagnoses and purport if there exists any correlation, and furthermore to build a predictive model that would help predict what kind of diagnosis a patient may encounter in the future by learning their historical diagnoses.

**Data Analysis:**
Plethora of data analytical tools were used in cleaning and transforming the data before modelling. Techniques like chi–squared, confusion matrix and recursive feature elimination were used to gain insights in the information provided by different features. The data available was categorical and before modelling was transformed into numerical data for easier analysis. Ordinal and Label encoding were used for this transformation. Interesting attributes like the age of the patient, the AMTS score, ASA grade, etc were used to find interesting trends.

**Machine Learning:**
Classification Machine Learning models like decision classifier, random forest, k-nearest neighbour, support vector machine, naïve bayes and logistic regression were used in building predictive models for the two objectives. These models were tuned by using gradient boosted algorithm and resampling of data. Different ML models reacted differently to different group of features and different train-test ratios.

**Objective I:**

Used two different final class labels for this objective.

Objective I (a) utilizes three class labels for prediction of the type of surgery required, and Objective I (b) utilizes seven class labels for the prediction of type of surgery required.

The final class labels of Obj I (a):

•	Arthroplasty

•	Internal Fixation

•	No operation required



The final class labels of Obj I (b) are the sub-types of the arthroplasty and internal fixation surgeries:

•	Arthroplasty Bipolar hemi

•	Arthroplasty Unipolar hemi

•	Internal Fixation – Sliding hip screw

•	Arthroplasty THR

•	Internal Fixation Screws

•	Internal Fixation nail (long and short)

•	No operation required

A confusion matrix for both Objective I (a) and Objective I (b) is attached as a png file. An AUC-ROC curve has also been plotted for three and seven class labels. They can be found at https://mohrayaanportfolio.wordpress.com/.

**Results of Objective I:**

•	86% of the intracapsular fractures were treated with arthroplasty, and 12% of the fractures were treated with internal fixation.

•	95% of the displaced – intracapsular fractures were treated with arthroplasty. There was almost the same number of arthroplasty and internal fixation operations performed on undisplaced – intracapsular fractures with 49% for arthroplasty and 47% for Internal fixation.

•	Patients suffered with an intertrochanteric fracture were heavily operated using internal fixation techniques. 97% of the intertrochanteric fractures were treated with internal fixation, further which 95% of the internal fixation methods used was SHS or sliding hip screw.

•	100% of all trochanteric and subtrochanteric fractures were treated with different subtypes of internal fixation. However, there have been different subtypes used for internal fixation with 60% of the subtrochanteric fractures being treated with IM nails and 40% were treated with SHS.

The best performing models for Objective I were Random Forest classifier and Gradient boosted model.
