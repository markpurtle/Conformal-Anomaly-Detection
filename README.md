# Conformal-Anomaly-Detection
3 month Master's Research Project undertaken at Royal Holloway, University of London

# Abstract
Anomalous samples appear in all types of datasets. These may be important samples
that require further attention, or unimportant samples that can be removed during
data cleaning. Therefore, it is desirable to provide automated, machine learning
methods to discover anomalies quickly. The objective of this project is to develop
and assess the use of conformal prediction as a basis for anomaly detection
algorithms. Anomaly detection using conformal prediction is a general method and
so can be applied to all types of datasets. It also has the benefit of a well-calibrated
false-alarm rate, so the user can intuitively alter the false alarm rate of the algorithm
to their desired maximum upper bound. In this project, conformal anomaly
detection is tested in the batch and online mode on the USPS handwritten digit
dataset with a number of added anomalies. Conformal anomaly detection shows
success at detecting these added anomalies, as well as anomalies that already existed
in the dataset. It also demonstrates the well-calibrated false alarm rate property of
conformal anomaly detection. The project extended into the problem of anomaly
detection in time series datasets, with the methods of conformal martingales and
conformal e-prediction with MUSUC. The two methods were tested on two
synthetic anomaly datasets and a real-world energy consumption dataset and their
results were compared. Both were successful at detecting the anomalies that existed
in these datasets. The main parameter of an anomaly threshold was varied, and the
two methods showed slightly different results. Generally, at lower thresholds, the
delay time to detecting the anomaly was lower and the MUSUC algorithm showed
slightly lower delay times compared to the conformal martingales. However, with
lower thresholds also came a greater number of false alarms and at almost all
thresholds, the MUSUC algorithm produced significantly more false alarms than
conformal martingales. Therefore, from these experiments, conformal martingales
appear to perform better overall as the false alarm rate is one of the biggest limiters
for anomaly detection algorithms. However, to see if this claim is true, further
experiments on a greater number of datasets and with alterations to the two
algorithms, such as different non-conformity measures, need to be tested. An
additional finding in this study was the use of a sliding window. The use of a sliding
window greatly improved the results of both algorithms on the energy consumption
dataset. However, it is unclear if this is a general improvement or specific to this
dataset without carrying out experiments on more real-world datasets. 

# My Code
I have presented the code I developed in a series of short Jupyter notebooks. Below
I will detail which notebooks correspond to which figures and the dataset files they used. 
When running the code, dataset files must be in the same directory as the Jupyter notebook. 

USPS Batch SVM Conformal Prediction.ipynb – Figure 7a, USPS dataset
USPS Batch 1NN Conformal Prediction.ipynb – Figure 7b, USPS dataset
USPS Online SVM Conformal Prediction.ipynb - Figures 8-13, USPS dataset
USPS Online ICAD SVM.ipynb – Figure 14, USPS dataset
USPS SVM Martingales.ipynb - Figure 15a and 16, USPS dataset
USPS 1NN Martingales.ipynb - Figure 15b, USPS dataset
NAB Jump Up Anomaly Results.ipynb - Figures 17, 18 and 19, NAB “Jump Up”
dataset
NAB Jump Up Martingale Changed Algorithm.ipynb - Figure 20, NAB “Jump Up”
dataset
NAB Jump Up MUSUC Changed Algorithm.ipynb - Figure 21, NAB “Jump Up”
dataset
NAB Jump Down Martingale.ipynb – Figure 22, NAB “Jump Down” dataset
NAB Jump Down MUSUC.ipynb – Figure 23, NAB “Jump Down” dataset
NAB No Anomaly.ipynb - Figures 26 and 27, NAB “Small Noise” No Anomaly
dataset
Energy Consumption Martingale.ipynb - Figure 28a, Energy Consumption dataset
Energy Consumption MUSUC.ipynb - Figure 28b, Energy Consumption dataset
Energy Martingales Sliding Window.ipynb - Figures 29 and 31, Energy
Consumption dataset
Energy MUSUC Sliding Window.ipynb - Figures 30 and 32, Energy Consumption
dataset
Energy Consumption Martingale Modification.ipynb – Figure 33, Energy
Consumption dataset 
50
Energy Consumption Random Shuffle.ipynb - Figures 34, 35, 36, Energy
Consumption dataset 
