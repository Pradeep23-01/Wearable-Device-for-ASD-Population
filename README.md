# Wearable-Device-for-ASD-Population
Designed an electronic module to measure the physiological signals of humans with which we collect physiological data from both ASD and Neurotypical people

## Summary:
Developed an IoT module that records physiological signals to assess emotions in ASD populations. Parameters such as heart rate, heart rate variation, electrodermal activity, and skin temperature were recorded from ASD and neurotypical populations. Machine learning algorithms were used to analyze the data and found notable differences between the two groups. The decision tree algorithm was found to provide better classification with an accuracy of 96.7%.

## Data Acquisition:
An electronic module was developed and used to collect data from both the ASD and neurotypical populations. The module was placed on the wrists of people with ASD to record data during various tasks. Some students were uncomfortable with the procedure which could have increased their anxiety. The same experiment was conducted with a neurotypical population of various age groups. Data was collected and stored in the module's storage device for later analysis.

## Data Processing:
The collected data is organized into a dataset and processed to remove extreme and redundant data. SpO2 values are removed, and BPM and GSR readings are considered. Human resistance is calculated from the GSR data using an equation. The processed dataset includes five features, age, gender, human resistance, BPM, and GSR readings for ASD and neurotypical people. Binary classification is performed using machine learning models to uncover relationships between the features and the target.

## Dataset Description:
The processed data is compared to typical physiological signal ranges, and SpO2 values are excluded as they were normal. Mean, standard deviation, minimum, and maximum values of BPM, GSR, and human resistance data are displayed in code(IFP_Visualize.ipynb) with their distributions. The ASD population's heart rate, GSR, and human resistance values are slightly higher than the neurotypical population, indicating differences in physiological parameters between the two populations that could aid in improving the machine learning classification task.

## Machine learning:
The study trained seven machine learning models, namely Logistic Regressor, SVM, Decision Trees, Random Forest, SGD, KNN, and Naive Bayes, on the dataset created from module readings of ASD and neurotypical people. Logistic Regressor, SGD, and SVM learned appropriate decision boundaries, while Decision Trees and Random Forest learned mappings through nodes in a tree structure. Naive Bayes used Bayes Theorem for classification, and KNN classified inputs based on the nearest neighbors in the dataset. The study compared the accuracy of the models trained with and without "Age" as a feature and compared them by plotting the corresponding ROC AUC curves.

## Conclusion:
The study found a significant difference in the distributions of data collected from ASD and neurotypical people based on the performance of the ML models. The study suggests that in the future, the collected data can be analyzed using deep learning algorithms to develop predictive analysis. The study also suggests the possible development of the module into a wearable device or tracker to monitor emotions and feed data to caretakers, parents, or concerned persons. Finally, the study notes that descriptive statistics from naturalistic data collection can aid in understanding the scenario.
