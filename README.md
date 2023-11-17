# Project3-identifying_keywords_in_a_speech
It contains file about this project

The goal was to produce a model wich will recognize some keywords during a speech. Those keywords were recorded by myself and were "green", "yellow", "red". I recorded 51 samples for each labels and I split the dataset with a 80/20 distribution. I put a NN classifier and before that a Mel Frequency Cepstral Coefficient (MFCC), that's globaly used for preparing audio datas. 

For my NN Classifier, I obtain a global accuracy of 78.7% (that's encouraging)  and a loss of 0.55. Actually, The Classifier did some errors with the yellow/green labels and the noise label. Some of yellows/greens are considered for him as noise. The red label isnt concerned about it. Maybe with more datas for each labels the score will improve easily.


For de the model testing, I got not the best results (~70%) but I decided next to this step to implement my model and try the keywords identification during a speech. 

After that, I deployed the model on the Arduino and I've tried my model with the example code. It works well, It would be intrusting to implement some led that will be on when the keyword concerned will be heard by the arduino, I'll try this.



Currently, Here's the Arduino library containing the model and an example of code using my model. 
