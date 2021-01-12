testing values:

conv + maxpool + without hide layer:
loss: 0.5038 - accuracy: 0.9470

conv + maxpool + 1 layer (512):
loss: 0.3535 - accuracy: 0.9262

conv + maxpool + 1 layer (384):
loss: 0.2462 - accuracy: 0.9424

conv + maxpool + 1 layer (320):
loss: 0.3035 - accuracy: 0.9295

conv + maxpool + 1 layer (256):
loss: 0.2109 - accuracy: 0.9535

conv + maxpool + 1 layer (192):
loss: 3.4966 - accuracy: 0.0557

conv + maxpool + 1 layer (128):
loss: 3.4922 - accuracy: 0.0572

conv + maxpool + 2 layer (256-256):
loss: 1.5176 - accuracy: 0.5209

conv + maxpool + conv + 1 layer (256):
loss: 0.1415 - accuracy: 0.9722

conv + maxpool + conv + maxpool + 1 layer (256):
loss: 0.3124 - accuracy: 0.9139

conv + conv + maxpool + 1 layer (256):
loss: 0.2036 - accuracy: 0.9611

conv + conv + conv + 1 layer (256):
loss: 0.1717 - accuracy: 0.9642

conv + maxpool + conv + conv + 1 layer (256):
loss: 0.1092 - accuracy: 0.9745

conv + maxpool + conv + conv + maxpol + 1 layer (256):
loss: 0.0627 - accuracy: 0.9860