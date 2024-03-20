##EmoAnalyzer  - ML project for speech based emotion detection

Detecting Emotions from Speech: A Machine Learning Project
This project explores using machine learning to analyze speech and recognize emotions. Our goal was to create a model that could understand the emotions behind everyday conversations, paving the way for more personalized experiences.

Understanding Audio Signals
We analyzed audio signals using concepts like prosody, which refers to the variations in pitch, loudness, and rhythm of speech that convey emotions.

Datasets and Audio Exploration
RAVDESS: This dataset provided a rich collection of audio recordings featuring various emotions like neutral, happy, sad, and angry.
SAVEE: This dataset offered additional speech samples with corresponding emotional labels.
We examined the audio files visually using waveforms and spectrograms to gain insights into their characteristics.

Feature Extraction with LibROSA
To train our model effectively, we extracted key features from the audio data. We used LibROSA, a Python library specifically designed for audio analysis. The features captured aspects like spectral energy and Mel-frequency cepstral coefficients (MFCCs), which provide information about the frequency content of the speech.

Building the Model: Convolutional Neural Networks
Given the classification nature of the problem (identifying emotions), we opted for Convolutional Neural Networks (CNNs) as our primary model architecture. We also experimented with Multilayer Perceptrons (MLPs) and Long Short-Term Memory (LSTM) networks, but they yielded lower accuracies.

Developing and fine-tuning the CNN model involved an iterative process. We began with a simpler architecture and gradually increased complexity while monitoring validation accuracy. The final model achieved over 70% accuracy in differentiating emotions.

Making Predictions
After training, we tested the model on unseen data. Here's a glimpse of the predicted emotions compared to the actual labels.

Live Voice Testing
To assess the model's generalizability, we recorded our own voices expressing different emotions and fed them into the model. The results demonstrated the model's ability to recognize emotions in live speech, as shown in the example where an angry male voice was correctly identified.

Decoding Model Outputs (0-9):

0 - Female Angry
1 - Female Calm
2 - Female Fearful
3 - Female Happy
4 - Female Sad
5 - Male Angry
6 - Male Calm
7 - Male Fearful
8 - Male Happy
9 - Male Sad
Conclusion
Building this model was an engaging challenge that involved experimentation and optimization. The model excels at distinguishing between male and female voices (100% accuracy) and achieves a respectable accuracy (over 70%) in emotion recognition. Further improvements can be made by incorporating a larger dataset for training.

