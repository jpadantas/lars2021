2021 Latin America Robotics SyposiumWinter Simulation Conference (WSC)

Python code for the paper Engagement Decision Support for Beyond Visual Range Air Combats.

This work aims to provide an engagement decision support tool for Beyond Visual Range (BVR) air combat in the context of Defensive Counter Air (DCA) missions. In BVR air combat, engagement decision refers to the choice of the moment the pilot engages a target by assuming an offensive stance and executing corresponding maneuvers. To model this decision, we use the Brazilian Air Force’s Aerospace Simulation Environment (Ambiente de Simulação Aeroespacial - ASA in Portuguese), which generated 3,729 constructive simulations lasting 12 minutes each and a total of 10,316 engagements. We analyzed all samples by an operational metric called the DCA index, which represents, based on the experience of subject matter experts, the degree of success in this type of mission. This metric considers the distances of the aircraft of the same team and the opposite team, the point of Combat Air Patrol, and the number of missiles used. By defining the engagement status right before it starts and the average of the DCA index throughout the engagement, we create a supervised learning model to determine the quality of a new engagement. An algorithm based on decision trees, working with the XGBoost library, provides a regression model to predict the DCA index with a coefficient of determination close to 0.8 and a Root Mean Square Error of 0.05 that can furnish parameters to the BVR pilot to decide whether or not to engage. Thus, using data obtained through simulations, this work contributes by building a decision support system based on machine learning for BVR air combat.

Please check the ipynb files:

* 1-Exploratory_Data_Analysis.ipynb: First overview in the dataset;
* 2-Feature_Engineering.ipynb: Feature engineering tecniques to create new features and figure out more information about the dataset;
* 3-Feature_Selection.ipynb: Feature selection techniques using ANOVA-f Statistic and Mutual Information Statistics;
* 4-XGBoost_Regression.ipynb: Extreme Gradient Boosting Regression Model.

There is no data folder because the missile launch data from the beyond visual range simulations was not allowed to be released at this moment.
