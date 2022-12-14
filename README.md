# Space-Weather-Detector
Symbolic AI algorithm to detect and approximate U-shape in spatial data spectograms

1. Dependencies:
  cv2
  numpy
  matplotlib.pyplot
  sklearn

2. Data:
  a set of spectrograms squared at size 224*224 pre-processed to be on grayscale.

3. Usage
  
  Algorithm:
  Apply the "detect" fonction on an image with the desired parameter.
  It use the "masker" function to create mask and find the most suitable one.
  The algorithm will threshold the image according to the parameter, create multiple mask and execute 
  a bitwise operation on them with each. The best mask (the one capturing the greatest part of the 
  U-shape if any) will be retained and the function return whether it fit between the floor and the ceil 
  and return a boolean of if it's a U-shape (1) or not (0) you can see the steps visually by uncommenting
  the result section but you will need to kill the jupyter kernell as there is too many image.
  
  Model:
  The parameters part of the model section serve to adjust the range on which the value will be trained on.
  the training part find the best parameter for the model but take a long time, I couldn't optimize it enough.
  
  Evaluation:
  The evaluation use the best parameters found during the training or you can just put the parameters
  commented manually if you don't want to wait for the model to train.
  
