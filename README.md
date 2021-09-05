Summary of the best struture search process.

The first structure I tried was "conv + maxpool + 1 layer (192)" as the handwritting.py example.
The next step was to try to increase the number of layers, with poor results. The conclusion was 
that the best model was one-layer.

Then the process was to adjust the number of cells and the initial image processing.


Finally the best model found was as follows:
testing values (dropout = 0.5):
conv + maxpool + conv + conv + maxpol + 1 layer (250):
loss: 0.0520 - accuracy: 0.9885



Summary of experienced models:

testing values (dropout = 0.5):

conv + maxpool + 1 layer (192):
loss: 3.4966 - accuracy: 0.0557

conv + maxpool + 1 layer (128):
loss: 3.4922 - accuracy: 0.0572

conv + maxpool + 2 layer (256-256):
loss: 1.5176 - accuracy: 0.5209

conv + maxpool + without hide layer:
loss: 0.5038 - accuracy: 0.9470

conv + maxpool + conv + maxpool + 1 layer (256):
loss: 0.3124 - accuracy: 0.9139

conv + maxpool + 1 layer (512):
loss: 0.3535 - accuracy: 0.9262

conv + maxpool + 1 layer (320):
loss: 0.3035 - accuracy: 0.9295

conv + maxpool + 1 layer (384):
loss: 0.2462 - accuracy: 0.9424

conv + maxpool + 1 layer (256):
loss: 0.2109 - accuracy: 0.9535

conv + conv + maxpool + 1 layer (256):
loss: 0.2036 - accuracy: 0.9611

conv + conv + conv + 1 layer (256):
loss: 0.1717 - accuracy: 0.9642

conv + maxpool + conv + 1 layer (256):
loss: 0.1415 - accuracy: 0.9722

conv + maxpool + conv + conv + maxpol + 2 layer (250 - 120):
loss: 0.1042 - accuracy: 0.9720

conv + maxpool + conv + conv + 1 layer (256):
loss: 0.1092 - accuracy: 0.9745

conv + maxpool + conv + conv + maxpol + 1 layer (192):
loss: 0.1149 - accuracy: 0.9749

conv + maxpool + conv + conv + maxpol + 1 layer (300):
loss: 0.1085 - accuracy: 0.9735

conv + maxpool + conv + conv + maxpol + 1 layer (240):
loss: 0.0973 - accuracy: 0.9812

conv + maxpool + conv + conv + maxpol + 1 layer (256):
loss: 0.0627 - accuracy: 0.9860

conv + maxpool + conv + conv + maxpol + 1 layer (250):
loss: 0.0520 - accuracy: 0.9885


dropout = 0.3
conv + maxpool + conv + conv + maxpol + 1 layer (250):
loss: 0.0954 - accuracy: 0.9812

dropout = 0.7
conv + maxpool + conv + conv + maxpol + 1 layer (250):
loss: 0.2504 - accuracy: 0.9381

* Change activation function from RELU to SIGMOID don't improve behavior