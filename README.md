# BR41n.io Hackathon - SSVEP Data Analysis 

![neurotechucb_small_transp](https://user-images.githubusercontent.com/41300679/141306168-ae07add5-cc00-4589-afe5-00e97bbc81ca.png?style=centerme)
![br41n io (1)](https://user-images.githubusercontent.com/41300679/139441793-fd89f9d0-b273-47bf-b252-3b36be58e1e1.png?style=centerme)

## Introduction
Held in Oct. 2021, the objective was to snalyze an SSVEP BCI data-set from a healthy person in order to optimize pre-processing, feature extraction and classification algorithms.

### Dataset
- We counted with 2 subjects, each one with 2 training sessions.
- The measures were made with 8 EEG channels.
- Each training session consisted of a LED blinking at differente frequencies: 15, 12, 10 and 9 [Hz].
- 256 Hz, filtered with a bandpass filter from 0.5-60 Hz, and a Notch filter of 50 Hz.

## Data Pre-processing
We start with raw data, passing thru a Bandpass filter from 0.5 to 60 Hz. Then a 50 Hz Notch filter processes de data. We then identify between target and non-target stimuli. We generate Epochs. Then, conatenate signal channels. Afterwards, we pass to standars scaling and end with PCA decomposition.

## Implementation
We tried several models to process the data:
- Distributed Random Forest
- Extremely Randomized Trees
- Extreme Gradient Boosting
- Deep Learning Tabular format.

## Results 
- We got the best reults with AutoML
