# Summer-research-
Summer research June 2020- September 2020. This repository contains code for the model and machine learning for growth control.
Different neural networks were used to arrive at the best perforning model. 
The cellular behaviour was modeled as a ODE and a initial model was set up to randomly generate data. ALL work was done in MATLAB.
Visit (https://netb.io/index.html) for more info.
We split the project into three steps, data, learning, and control. 
1.	Data: We started off by generating data using an ordinary differential equation model with constant inputs using MATLAB. We then added time 
varying inputs where our output was protein expression rate. 

2.	Learning: Next, we used a static model to allow learning tohappen and to verify that the system is working as necessary. Next, we perturbed
the model by disturbing it a little bit in different ways and allowed learning to happen again, this caused the error to be very high to begin 
with and then gradually decrease as the neural net learns again. 

3.	Control: The goal for the control part was to achieve a desired expression rate which was in bounds with our training set. We did this by 
generating a set of inputs to forecast the next desirable value of expression rate. We only did this for a single time step in the future. 
It would be more ideal to do it for multiple time steps in the future, however, the data grows exponentially so it was very difficult to do 
so on our PCs since we had no access to labs. Next, once a desirable input is found, we commit it to our neural net and continue the process 
until the output converges to the value we want.
