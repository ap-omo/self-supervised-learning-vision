# MPP: Locally self-supervised deep learning for vision

The aim of this project is to develop a biologically inspired approach to deep learning for computer vision. The core premise of this project is that biological neural systems do not learn through global error backpropagation, like artificial neural networks (ANNs) do, but instead on local, self-supervised learning rules.


This repository consists of:

- A detailed project report with over 10,000 words covering the important aspects of the major project
- A project outline written before the beginning to make the intended outcome and motive clear

- A short description of the setup used throughout the duration of the project
  - All code was ran using Visual Studio Code through WSL2 on a Windows machine instead of the standard choice of native Linux
  - For the purpose of recreation, guidance regarding setup on a Windows 10 machine and its prerequisites are provided

- Other documentation regarding the mechanisms of the functions and classes included in Tensorflow/Keras
  - Exploring how the main functions and classes work together in machine learning
  - Records of the effect of changing certain values (such as hyperparameters) and activation functions etc. on the final output
  - Explanation of why certain functions and classes were/weren't suitable for the task given

- Various models grouped by type and level
  - Models improved over time, with each revision improving the output/efficiency of the model
  - Improved revisions of models documented in their respective folders with README.md
  
- A fully functional finalised model which most importantly makes use of local, self-supervised learning rules
  - The model is therefore (somewhat) biologically plausible as it still produces a decently high standard of output
  - Achieves the goal outlined at the beginning of the project
