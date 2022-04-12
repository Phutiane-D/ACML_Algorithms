# ACML_Algorithms

Investigating practical aspects of machine learning to a problem that interests us. As part of this project, we are required to do a presentation (no longer than 10 mins) and report our findings in a scientific paper format. 

## Algorithms to investigate

1. Logistic regression
2. Forgot the other 1

### Dataset

The dataset used in this project comes from kaggle.com. It was uploaded by Kory Becker
and is licensed under the creative commons. The raw data for this dataset was compiled
from:
● The Harvard-Haskins Database of Regularly-Timed Speech

● Telecommunications & Signal Processing Laboratory (TSP) Speech Database at
McGill University, Home
● VoxForge Speech Corpus, Home
● Festvox CMU_ARCTIC Speech Database at Carnegie Mellon University

The raw data was then processed by acoustic analysis in R using the seewave and tuneR packages, with an analyzed frequency range of 0hz-280hz to produce the final dataset.

### What are the attributes? What are the targets?
The attributes in the dataset consist mainly of derived statistical features of each recorded voice sample. 
These attributes include:
● meanfreq: mean frequency i.e the average across the entire frequency signal(in kHz)
● sd: standard deviation of frequency

● median: median frequency (in kHz)

● Q25: first quantile (in kHz)

● Q75: third quantile (in kHz)

● IQR: interquartile range (in kHz)

● skew: skewness

● kurt: kurtosis

● peakf: peak frequency (the highest pitched sound in the recording)

● mode: mode frequency

● sp.ent: spectral entropy

● sfm: spectral flatness

● mode: mode frequency

● centroid: frequency centroid (see specprop)

● peakf: peak frequency (frequency with highest energy)

● meanfun: average of fundamental frequency measured across acoustic which is equivalent to average pitch

● minfun: minimum fundamental frequency measured across acoustic signal

● maxfun: maximum fundamental frequency measured across acoustic signal

● meandom: average of dominant frequency measured across acoustic signal

● mindom: minimum of dominant frequency measured across acoustic signal

● maxdom: maximum of dominant frequency measured across acoustic signal

● dfrange: range of dominant frequency measured across acoustic signal

● modindx: modulation index. Calculated as the accumulated absolute difference between adjacent measurements of fundamental frequencies divided by the
frequency range

● label: male or female

### How many data points do you have?
3,168 data points. There are no null values in the dataset.

### How balanced are the classes?
The two classes are balanced evenly. 1584 data points are labelled as female, the other
1584 data points are labelled as male.

### State what you are trying to predict with the data?
Given a recorded voice sample for a human speaker that is represented as a set of acoustic features stated as numeric values, we are trying to predict the sex of the speaker in the sample.
