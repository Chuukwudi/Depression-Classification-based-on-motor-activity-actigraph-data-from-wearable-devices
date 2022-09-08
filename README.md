# Depression diagnosis using motor activity / actigraph data from wearable devices

## About the data

Data used was downloaded from [this website](https://datasets.simula.no/depresjon/#download) and was
sourced from smart actigraph wrist watches belong-
ing to 55 different individuals out of which 23 were
unipolar bipolar and depressed patients, and 32 were
healthy people. This actigraph wristwatch takes pa-
tients health details such as patients motor activity,
sleep/inactivity and heart rate. In this case, each wear-
able device/observation is a CSV file that contains the
following columns:
1. timestamp (one minute intervals)
2. date (date of measurement)
3. activity (activity measurement from the actigraph watch).

The data set is already separated into two folders,
containing actigraph data (CSV files) of patients col-
lected over time. The first group is stored in a folder
called "condition", which contains actigraph data of 23
depressed patients who suffer from bipolar/unipolar.
In contrast, the second folder, "control", contains acti-
graph data of 32 regular people with no signs of depression.
For every sample, actigraph data is taken every
minute, making it 1440 observations(minutes) in one day.

## Data Processing and preparation
Details can be found [here](https://github.com/Chuukwudi/Depression-Classification-based-on-motor-activity-actigraph-data-from-wearable-devices/blob/main/Chukwudi_Ajoku_A0151658_Report.pdf).

## Models used:
The models used were;
1. K Nearest Neighbors
2. Linear Support Vector Machine(SVM)
3. RBF SVM
4. Gaussian Process
5. Decision Trees
6. Random Forest
7. AdaBoost
8. Naive Bayes
9. Quadrant Discriminant Analysis
10. Deep Neural Networks.

### The 3 best models were:
#### Random Forest:
Random forest is a very robust classification algorithm
because it is not prone to over-fitting. Further more, be-
cause it is a tree based algorithm, it is can automatically
handle datasets with imbalanced classes as evidenced
above.

#### Gaussian Process:
Gaussian Processes is known to perform wonderfully for time series related data(Roberts et al., 2012;
Wikipedia, 2021). It is based on Gaussian (Normal) distribution and as such, inherits its properties as well.
This was a big advantage.

#### Neural Networks:
The main advantage Neural Networks had was its ability to model non-linear and complex relationships.
However, the model did not do as well as expected because of few data. Neural Networks work best with very large data.