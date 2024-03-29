# Frame-Level-Speech-Recognition

# Part 1 : Creating a basic MLP

In Part 1, we create the core components of multilayer perceptrons: linear layers, activations, loss functions, and batch normalization. 
We implement these classes in MyTorch, our own deep learning library inspired by PyTorch.
The task is to specifically implement the mathematics into code, and understand how all the components are related. 
(<ins>Note</ins>: we use "numpy" and no other python library)

# Part 2 : Frame Level Classification of Speech

In this project, we take our knowledge of feedforward neural networks and apply it to a more useful task than recognizing handwritten digits; speech recognition. 

<ins>Task</ins> : to generate predictions for the phonemes of the test set. 

<ins>Evaluation Metric</ins> : based on the accuracy of the prediction of the phoneme state labels for each frame in the test set. 

<ins>Dataset</ins> : audio recordings (utterances) and their phoneme state (subphoneme) labels. The data comes from articles published in the Wall Street Journal (WSJ) that are read aloud and labelled using the original text. 

![1p2_1](https://user-images.githubusercontent.com/92863991/212860866-51a2caec-b7f1-4c7d-881b-b99fab3a813a.png)

<ins>The training data comprises of</ins>:

• Speech recordings (raw mel spectrogram frames)

• Frame-level phoneme state labels
  

<ins>The test data comprises of</ins>:

• Speech recordings (raw mel spectrogram frames)

• Phoneme state labels are not given


![1p2_2](https://user-images.githubusercontent.com/92863991/212860863-96c2707c-54da-4e62-8fd1-3346584f9441.png)


Our objective is to identify the phoneme state label for each frame in the test data set. It is important to note that utterances are of variable length.

<ins>Workflow</ins> : 

![1p2_4](https://user-images.githubusercontent.com/92863991/212860876-7f46e9dd-10b5-4a61-97a7-c8e3f541f272.png)
