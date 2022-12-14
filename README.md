# Space-Weather-Detector
Symbolic AI algorithm to detect and approximate U-shape in spatial data spectograms

1. Dependencies:
  cv2
  numpy
  matplotlib.pyplot
  sklearn

2. Data:
  a set of spectrograms squared at size 224*224

3. Usage
  
  Algorithm:
  Apply the "detect" fonction on an image with the desired parameter.
  It use the "masker" function to create mask and find the most suitable one.
  
  Model:
  The parameters part of the model section serve to adjust the range on which the value will be trained on.
  the training part find the best parameter for the model but take a long time, I couldn't optimize it enough.
  
  Evaluation:
  The evaluation use the best parameters found during the training or you can just put the parameters
  commented manually if you don't want to wait for the model to train.
  
