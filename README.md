# Signal Modulation Detection using Conv1D
 Classification of signals based on its modulation

## Overview
The jupyter notebook generates signals modulated with Bi-Phase Shift Keying (BPSK) and Linear Frequency Modulation (LFM). <br>

Modulation | Characteristics
-----------|-----------------
BPSK       |Change in phase of signal by a magnitude of 𝜋 
LFM        |Constant change in frequency

The neural network will learn to classify 3 different input signals, Continuous Wave (CW), BPSK and LFM.
This is achieved through Keras 1D convolutional networks.  <br>

### Test Conditions
Using Scipy and Numpy, signals of various phase shifts and sweep rates were synthesised.

Characteristic               |Range
-----------------------------|------
Frequency Sampling           |1280MHz
Frequency                    |160MHZ – 600MHZ
Phase Shift                  |±𝜋
Sweep Rate                   |1MHZ – 400MHZ
SNR                          |-10dB – 10dB
Time                         |1𝜇𝑠

## Results
After 200 epochs, the accuracy was around 90%, this may be attributed to the ideal conditions of the signal.
Further improvements can be made by training the data on more unique data such as real signal environments.
Work could also be done to measure the sensitivity of the neural net and measures its performance over 
different SNR and sweeps rates to study the neural net's limitations and suggest improvements. <br>

![alt text](Accuracy.png "Accuracy of Neural Net") ![alt text](Loss.png "Is this loss?")




## Dependencies
Pandas <br>
Numpy <br>
Scipy <br>
Matplotlib <br>
Keras <br>
Sklearn <br>

