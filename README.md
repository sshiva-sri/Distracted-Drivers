# Distracted-Drivers
Distracted Driver MultiAction Classification

Problem statement: According to the CDC motor vehicle safety division one in five car accidents is caused by a distracted driver. Sadly, this translates to 425,000 people injured and 3,000 people killed by distracted driving every year. State Farm hopes to improve these alarming statistics, and better insure their customers, by testing whether dashboard cameras can automatically detect drivers engaging in distracted behaviors. Given a dataset of 2D dashboard camera images, Are they driving attentively, wearing their seatbelt, or taking a selfie with their friends in the backseat?


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


Solution & Experiments: 

Using tensorflow, Keras, Conv2D, MaxPooling2D.
•	Epochs=10, took 1.5hours to train the model with GPU, got an accuracy of 96.7%.
•	Epochs=20, took 2.3hours to train the model with GPU, got an accuracy of 97.2%.

Using tensorflow, Keras, Conv2D, MaxPooling2D, Dropout, BatchNormalization.
•	Epochs=10, took 30min to train the model with GPU, got an accuracy of 98%.
•	Epochs=20, took 1hour to train the model with GPU, got an accuracy of 99.5%.


Performance: Final Accuracy(evaluate_generator) is 95.5%.
