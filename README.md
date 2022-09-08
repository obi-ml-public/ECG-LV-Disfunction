# ECG-LV-Disfunction
Model to detect LV disfunction from ECG

# Environment
- tensorflow 2.4.1 
- numpy 1.19.2
- pandas 1.3.4

# Requirements
Put the input file in the same directory as EFcode_1220.py as numpy array.
The input should be formated as a 3d numpy array with shape 2500,12,1 (time,induction,1).
The ECG should be in 250 Hz recording with voltage unit = mV.

# Weights
The model weights are not publicly available because it may contain patient information.
The web interface to run the full model is available at http://onebraveideaml.org/

# Model architecture
The model consists of 20 layers of multi_conv2D module, which consists of 3 different-depth 2D convolutional layers.
The model has 258,754,113 parameters (258,546,625 trainable)
