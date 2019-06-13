# Distracted-Drivers
Distracted Driver MultiAction Classification

Problem statement: 
-------------------
According to the CDC motor vehicle safety division one in five car accidents is caused by a distracted driver. Sadly, this translates to 425,000 people injured and 3,000 people killed by distracted driving every year. State Farm hopes to improve these alarming statistics, and better insure their customers, by testing whether dashboard cameras can automatically detect drivers engaging in distracted behaviors. Given a dataset of 2D dashboard camera images, Are they driving attentively, wearing their seatbelt, or taking a selfie with their friends in the backseat?


c0: safe driving

c1: texting - right

c2: talking on the phone - right

c3: texting - left

c4: talking on the phone - left

c5: operating the radio

c6: drinking

c7: reaching behind

c8: hair and makeup

c9: talking to passenger

-----------------------------------------------------------------------------------------------

Initial proposal for solution:
------------------------------
Built a simple Neural Network CNN with Keras with 3 convolutions ,3 Maxpooling ,1 Flatten and 3 Dense layers.

Parameters calculation:
___________________________

No of parameters = Input layer * 	filter size * no of filters + bias
____________________________________________________________________
conv2d_1 	params=320

1 * 3 * 3 * 32 + 32 =320
___________________
conv2d_2 	params=18496

32 * 3 * 3 * 64 + 64 =18496
____________________
conv2d_3 	params=73856

64 * 3 * 3 * 128 + 128=73856
____________________
max_pooling2d_3 (MaxPooling2 (None, 30, 30, 128)       

flatten_1 (Flatten)          (None, 115200)           

30 * 30 * 128 = 115200
______________________________________________
 dense_1 (Dense)              (None, 512)               58982912  

115200 * 512 + 512 = 58982912
_________________________


Problems Faced:
---------------
* Main problem faced was 4GB RAM was not sufficient, system got struck once started with the training the model. 

*So tried processing in Kaggle Kernel. Training the model utilized 12.5GB of RAM and the training time was 30minutes.

*Initial Accuracy was just 10% .


Experiments:
-------------



Final model code:
-----------------



Performance:
------------

Final Accuracy is 99.51%



Saved Models: 
-------------





Performance: Final Accuracy(evaluate_generator) is 99.5%.
