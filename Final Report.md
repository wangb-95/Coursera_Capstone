# Seattle: Understanding The street design, Driver Behavior and the Surrounding Environment Contribute to Crashes
## 1 Intruduction / Business Problem
All around the world, roads are shared by many motorized vehicles that have made transportation faster and more comfortable while supporting many countries’ economic and social development. However, these vehicles cause a global problem. Car accidents are responsible for 1.35 million deaths on roadways every year. Almost 3,700 people are killed globally in road traffic crashes, where more than half of those killed are pedestrians, motorcyclists, and cyclists.

While Seattle has seen a 30 percent decline in traffic fatalities over the last decade, traffic collisions are still a leading cause of death for Seattle residents age 5 to 24. Older adults are also disproportionately affected, so this trend could grow as the population ages. To supplement the findings of the City’s Bicycle and Pedestrian Safety Analysis project and provide policy makers and engineers with actionable information for developing and implementing interventions, we need have a deeper study for Collision data from Seatle. 

The objective of this project is to define the problem, to find the factors that can have a relevant weight in the quantity and seriousness of the accidents, so that any organism, company or enterprise interested in reducing these figures, can focus the resources in points where these conditions converge.

My study will focus in three part: 
    1. How street design impact collisions possibility 
    2. How the Surrounding Environment Contribute to Crashes
    3. How the Driver Behavior contributes to Crashes
    4. What is the most correlative factor? 


## 2 Data
### 2.1 Data description 
For an accurate prediction of the magnitude of damage caused by accidents, they require a large number of reports on traffic accidents with accurate data to train prediction models. The data set provided for this work allows the analysis of a record of 200,000 accidents in the state of Seattle, from 2004 to the date it is issued, in which 37 attributes or variables are recorded and the codification of the type of accident is allowed, grouped according to 84 codes. The information can be extracted from it:
  1. Weather 
  2. Road Condition
  3. Light Condition 
  4. Speeding
  5. The consequence of accidents : Fatalities, Injuries, etc

However, for this case study, not all the attributes are useful as the main objective is to predict an accident’s probability and severity. Therefore, the Dataset needs deep understanding and analysis before choosing the right attributes to reach our goal.

For example, SDOTCOLNUM, X, Y, LOCATION, INCDTTM, INCDATE, REPORTNO, COLDETKEY, INCKEY and OBJECTID are features that give descriptive and detailed information about an accident, and are then not relevant to predict the severity of an accident in general.

Moreover, EXCEPTRSNCODE, EXCEPTRSNDESC, PEDROWNOTGRNT, SPEEDING, INATTENTIONIND and INTKEY have a high number of missing data that would skew and bias our predictive model.
After selecting the appropriate features, the new Dataset is balanced and preprocessed before feeding it to a supervised machine learning model that will learn to predict in the future the probability of a car accident.

## Methodology 
