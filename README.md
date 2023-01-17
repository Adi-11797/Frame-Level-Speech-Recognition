# Frame-Level-Speech-Recognition

# Part 1


# Part 2 : Frame Level Classification of Speech

In this project, we take our knowledge of feedforward neural networks and apply it to a more useful task than recognizing handwritten digits; speech recognition. 

Task : to generate predictions for the phonemes of the test set. 

Evaluation Metric : based on the accuracy of the prediction of the phoneme state labels for each frame in the test set. 

Dataset : audio recordings (utterances) and their phoneme state (subphoneme) labels. The data comes from articles published in the Wall Street Journal (WSJ) that are read aloud and labelled using the original text. 

The training data comprises of:
• Speech recordings (raw mel spectrogram frames)
• Frame-level phoneme state labels
The test data comprises of:
• Speech recordings (raw mel spectrogram frames)
• Phoneme state labels are not given
Our objective is to identify the phoneme state label for each frame in the test data set. It is important to note that utterances are of variable length.
