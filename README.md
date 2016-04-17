# lstm-biology

Code and report for my project **"Applying LSTM neural networks to biological cell movement"** at the [Biophysics Group](http://lpmt.biomed.uni-erlangen.de/group) of the University of Erlangen-Nuremberg.

**Abstract:** Neural networks with Long Short-Term Memory (LSTM) were used on scientific time series 
data. Each time series contains the positions of a biological cell while it moves through one 
of three environments (a collagen network, a plastic surface, or a plastic surface coated with 
fibronectin). The networks were used for two tasks: 1) Classifying the movement trajectories 
based on the cell environment. Several networks of increasing complexity were trained on 
parts  of  the  trajectories,  using  softmax  classification.  The  best  networks  achieved  an 
accuracy of ~95 % (on test data) and generalized well to longer trajectories. 2) Generating 
new  movement  trajectories  by  predicting  one  step  of  a  time  series  after  another.  For  this 
purpose, LSTM was combined with the idea of a mixture density network (MDN): It does not 
predict  the  values  of  the  next  time  step  directly,  but  outputs  the  parameters  of  a  mixture 
distribution,  from  which  they  can  be  sampled.  The  generated  trajectories  replicated  the 
shape as well as the rough statistics of the original dataset.  
