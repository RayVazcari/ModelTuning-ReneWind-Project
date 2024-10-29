<h1><center><font size=10>Data Science and Business Analytics</center></font><p
<center>Project 6 - Model Tuning - Classification model to identify Mechanical Failures for ReneWind</center></h1><p

<p align="left"> 
  <a href="https://github.com/RayVazcari?tab=followers">
    <img alt="followers" title="Follow me on Github" src="https://custom-icon-badges.demolab.com/github/followers/RayVazcari?color=236ad3&labelColor=1155ba&style=for-the-badge&logo=person-add&label=Follow me on Github &logoColor=white"/></a>
  <a href="https://www.linkedin.com/in/rayvazcari/">
    <img alt="Linkedin Profile" title="Linkedin Profile" src="https://custom-icon-badges.demolab.com/badge/-Linkedin%20Profile-blue?style=for-the-badge&logoColor=white&logo=linkedin"/></a>
</p>

---

**`| Supervised Learning | Data Visualization | Python | Data Cleaning | Univariate Analysis & Multivariate Analysis | Data Preprocessing | Exploratory Data Analysis (EDA) | Customer Profiling | Bagging Classifiers (Bagging, Random Forest) | Boosting Classifiers (AdaBoost, Gradient Boosting, XGBoost) | Hyperparameter Tuning with GridSearchCV | Upsampling | Downsampling | Regularization Techniques |`**

---

### 🧰 Languages Libraries and Tools I Used on This Project
<a href="https://jupyter.org/" target="_blank"><img align="left" alt="Jupyter" title="Jupyter" width="30px" style="padding-right:10px;" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/jupyter/jupyter-original-wordmark.svg" /></a>
<a href="https://matplotlib.org/" target="_blank"><img align="left" alt="Matplotlib" title="Matplotlib" width="30px" style="padding-right:10px;" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/matplotlib/matplotlib-original.svg" /></a>
<a href="https://numpy.org/" target="_blank"><img align="left" alt="Numpy" title="Numpy" width="30px" style="padding-right:10px;" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/numpy/numpy-original.svg" /></a>
<a href="https://pandas.pydata.org/" target="_blank"><img align="left" alt="Pandas" title="Pandas" width="30px" style="padding-right:10px;" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/pandas/pandas-original.svg" /></a>
<a href="https://plotly.com/" target="_blank"><img align="left" alt="Plotly" title="Plotly" width="30px" style="padding-right:10px;" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/plotly/plotly-original.svg" /></a>
<a href="https://www.python.org/" target="_blank"><img align="left" alt="Python" title="Python" width="30px" style="padding-right:10px;"  src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/python/python-original.svg" /></a>
<a href="https://code.visualstudio.com/" target="_blank"><img align="left" alt="VScode" title="VScode" width="30px" style="padding-right:10px;"  src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/vscode/vscode-original.svg" /></a>
<a href="https://seaborn.pydata.org/" target="_blank"><img align="left" alt="Seaborn" title="Seaborn" width="30px" style="padding-right:10px;" src="https://seaborn.pydata.org/_images/logo-mark-lightbg.svg" /></a>

<br />

---

### **Project Overview**

In this project, I developed and tuned machine learning models to predict potential failures in wind turbine generators, providing ReneWind with a tool to enhance their predictive maintenance strategy. With sensor data from turbine components and environmental conditions, I aimed to accurately identify generators at risk of failure, allowing the company to address issues proactively, reduce downtime, and lower maintenance costs.

I began by performing Exploratory Data Analysis (EDA) to understand patterns within the data, particularly focusing on the target variable distribution. Given the class imbalance—where failure cases were outnumbered by non-failure cases—I applied upsampling and downsampling techniques to ensure the model could learn effectively from both classes without bias toward the more common non-failure cases.

Following data preprocessing, I built a variety of classification models, experimenting with regularization techniques to prevent overfitting and improve model generalization. These models included Logistic Regression with L2 regularization as a baseline and advanced classifiers like Random Forest and Gradient Boosting, which offered ensemble learning benefits for higher predictive accuracy.

For model selection, I used GridSearchCV for hyperparameter tuning, allowing me to optimize parameters such as the depth of decision trees, the number of estimators, and regularization strength. This tuning process maximized the models’ predictive performance, enhancing their ability to correctly classify true positives (TP) and avoid costly false negatives (FN), which represent undetected failures that could lead to expensive generator replacements.


### **Summary of Findings**

- `Predictive Accuracy in Identifying Failures`: Through extensive tuning of ensemble models like Random Forest and Gradient Boosting, the final model achieved a high level of accuracy in predicting generator failures. The model showed strong performance in distinguishing between failure (1) and non-failure (0) cases, with an emphasis on correctly identifying True Positives (TP)—actual failures detected by the model. This ensures that critical failures are flagged early, enabling proactive repairs.
- `Minimizing Costly False Negatives`: Given the higher financial impact of False Negatives (FN) (where actual failures are undetected by the model, potentially leading to expensive generator replacements), I focused on model strategies that reduce this error type. The model's tuning process prioritized recall, ensuring a lower rate of FNs. This approach reduces replacement costs by catching failures that can be addressed with repairs, which are less expensive and prevent complete generator breakdowns.
- `Managing False Positives to Optimize Maintenance Costs`: While minimizing FNs was crucial, I also focused on controlling False Positives (FP)—instances where the model incorrectly predicts a failure, prompting unnecessary inspections. Although inspection costs are lower than repair costs, they can add up over time. By fine-tuning model thresholds and regularizing the model, I struck a balance that minimizes FPs, ensuring that the maintenance team is not burdened with excessive inspection tasks.
- `Impact of Environmental and Component-Specific Variables`: EDA revealed that certain sensor variables related to environmental factors (like temperature, humidity, and wind speed) and specific turbine components (such as gearbox and blade status) were highly indicative of potential failures. These features played a prominent role in the final model, highlighting the conditions and parts most susceptible to wear or failure, allowing ReneWind to better understand operational risks and address them preemptively.
- `Model Robustness Through Regularization`: Regularization techniques, particularly in ensemble models, proved essential in preventing overfitting, ensuring that the model performs consistently well on both training and testing datasets. This robustness is vital for deployment in real-world scenarios, where sensor data conditions can vary widely across turbines and environments.

### **Impact**

The final model provides ReneWind with a robust predictive maintenance solution, optimizing maintenance schedules to address issues before costly failures occur. By minimizing the occurrence of undetected failures (FN), this solution significantly lowers replacement costs, and by controlling false positives (FP), it reduces unnecessary inspections, balancing cost efficiency with operational accuracy.

### **Project Outcome**

Through this project, I refined my skills in handling imbalanced data, ensemble modeling, and hyperparameter tuning. The model demonstrates how machine learning can be applied to industrial maintenance, underscoring the potential for predictive analytics to drive cost savings and operational improvements in renewable energy.

<br />

---

<center><img src="https://renewind.be/web/image/622-51ef1e37/logo%20renewind-vect-v2.png"></center>

---

---

### Business Context

Renewable energy sources play an increasingly important role in the global energy mix, as the effort to reduce the environmental impact of energy production increases.

Out of all the renewable energy alternatives, wind energy is one of the most developed technologies worldwide. The U.S Department of Energy has put together a guide to achieving operational efficiency using predictive maintenance practices.

Predictive maintenance uses sensor information and analysis methods to measure and predict degradation and future component capability. The idea behind predictive maintenance is that failure patterns are predictable and if component failure can be predicted accurately and the component is replaced before it fails, the costs of operation and maintenance will be much lower.

The sensors fitted across different machines involved in the process of energy generation collect data related to various environmental factors (temperature, humidity, wind speed, etc.) and additional features related to various parts of the wind turbine (gearbox, tower, blades, break, etc.).

### Objective

“ReneWind” is a company working on improving the machinery/processes involved in the production of wind energy using machine learning and has collected data of generator failure of wind turbines using sensors. They have shared a ciphered version of the data, as the data collected through sensors is confidential (the type of data collected varies with companies). Data has 40 predictors, 20000 observations in the training set and 5000 in the test set.

The objective is to build various classification models, tune them, and find the best one that will help identify failures so that the generators could be repaired before failing/breaking to reduce the overall maintenance cost.
The nature of predictions made by the classification model will translate as follows:

- True positives (TP) are failures correctly predicted by the model. These will result in repairing costs.
- False negatives (FN) are real failures where there is no detection by the model. These will result in replacement costs.
- False positives (FP) are detections where there is no failure. These will result in inspection costs.

It is given that the cost of repairing a generator is much less than the cost of replacing it, and the cost of inspection is less than the cost of repair.

“1” in the target variables should be considered as “failure” and “0” represents “No failure”.

### Data Description

- The data provided is a transformed version of original data which was collected using sensors.
- `Train.csv` - To be used for training and tuning of models.
- `Test.csv` - To be used only for testing the performance of the final best model.
- Both the datasets consist of 40 predictor variables and 1 target variable
