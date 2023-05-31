# Music-Genre-Classification
Deep learning algorithms such as CNN and RNN have played a major role in acoustic modeling in recent years. In this project, different features of audio files are explored. Both deep learning and classical machine learning algorithms are used to map the extracted features from music files to their respective genre.  Specifically, SVM, XGBoost, CNN, LSTM and ResNet50 are used to match the patterns in the feature space to a specific genre. Pushing the accuracy measure of the current SOTA is also an objective. The features were extracted from the available GTZAN music dataset and exploratory data analysis was performed for the same. The models were then trained and evaluated the performance using common performance matrices against the XGBoost baseline model.

The problem at hand is to develop an accurate music genre classification model using Machine Learning and Deep Learning algorithms. The goal is to train audio datasets for this purpose and compare the performance of different models with a Baseline model. 

In this project, two types of models were trained for both SVM and XGBoost based on the extracted features. First, the models were trained by reading the audio files as Mel Spectrograms, and a SVM with a linear kernel and XGBoost were used to obtain a baseline result. For the second type of classical machining learning algorithms, an SVM model and an XGBoost model was used again but this time a Grid Search optimization method was used to help select the most important features and hyperparameters. The XGBoost model for Mel Spectrogram is chosen as  the baseline model.

For the deep learning models, 2D CNN, LSTM, and ResNet50, the audios are read as Mel Spectrograms and split into 1.5 second windows with 50% overlapping, resulting in a dataset with samples x time x frequency x channels shape.

Standard performance metrics like the Confusion Matrix, Accuracy score, Precision score, Recall score, and F1 score were used to evaluate different models used in this task. 


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

**MODEL TRAINING**
- Run the code **handcrafted_features.ipynb** to extract the audio features and the classical machine learning models( SVM and XGBoost) for combined features.
- Run the code **SVM_mel.ipynb** and **XGB_mel.ipynb** to run the classical machine learning models using Mel spectogram features.
- Run the codes **CNN.ipynb** , **lstm.ipynb**, **resnetv3.ipynb** to run the deep learning models using Mel spectrogram features.

**Inference**
Compared to our baseline model (XGBoost-Mel Spectrogram model), the 2D CNN model with 6 layers outperformed all other algorithms with an accuracy score of 76%. 
