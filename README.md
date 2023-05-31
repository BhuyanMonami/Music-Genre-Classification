# Music-Genre-Classification
Deep learning algorithms such as CNN and RNN have played a major role in acoustic modeling in recent years. In this project, different features of audio files are explored. Both deep learning and classical machine learning algorithms are used to map the extracted features from music files to their respective genre.  Specifically, SVM, XGBoost, CNN, LSTM and ResNet50 are used to match the patterns in the feature space to a specific genre. Pushing the accuracy measure of the current SOTA is also an objective. The features were extracted from the available GTZAN music dataset and exploratory data analysis was performed for the same. The models were then trained and evaluated the performance using common performance matrices against the XGBoost baseline model.

Music genre classification is utilized by music streaming services to recommend songs to listeners. By analyzing the genre of a listener’s preferred music, the streaming service can suggest new songs that match the same genre. Music genre classification also assists in analyzing music trends and patterns. However, as music has evolved over time, and the quantity has surged rapidly, classification of music genres is a challenging task. Most of the music genre annotation is being done manually. However, one can leverage ML and AI technologies to assist or replace the manual processes. 

The problem at hand is to develop an accurate music genre classification model using Machine Learning and Deep Learning algorithms. The goal is to train audio datasets for this purpose and compare the performance of different models with a Baseline model. The challenge is to identify the most effective algorithm for this task, given the subjective nature of music and the potential overlap between some genres. The ultimate objective is to push the accuracy measure of the current state-of-the-art in music genre classification models. Standard performance metrics like the Confusion Matrix, Accuracy score, Precision score, Recall score, and F1 score were used to evaluate different models used in this task. 


**DATA** : The GTZAN dataset can be found in the **data** directory of this project. The structure should look like this:

    ├── data/

        ├── genres
   
      ├── blues
      
      ├── classical
      
      ├── country
      
      .
      
      .
      
      .
      
      ├── rock
