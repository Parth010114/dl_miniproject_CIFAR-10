# Introduction
In our image classification project, we used the ResNet architecture which has residual blocks and skipped connections, allowing for a deeper network than other classification architectures. However, we wanted to keep our model's parameter count under 5 million, so we changed the depth of some residual blocks. We discovered that increasing the depth in blocks with a high number of channels did not improve learning. We also attempted to increase the number of layers skipped in each residual block, but this did not improve performance. Therefore, we did not include it in our final model.
We used kernel sizes of 3 and 5 in our experiments, but they had no significant impact on the precision of our model. But we discovered that changing the learning rate had a big impact on accuracy, with lower rates leading to higher accuracy. Then, by repeatedly looping through plausible inputs, we calculated programmatically the optimal values for the hyperparameters block layer depth, learning rate, and stride. An accuracy of 93.95 percent was attained after testing.

Submitted By:

Ishwant Singh Bhayana (isb5064@nyu.edu) 
Prajna Ravindra Nayak (pn2224@nyu.edu)
Parth Mehta (pjm9767@nyu.edu) 
