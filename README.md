# MusicGenreClassifier_MiniProject

A music genre classifier using classic machine learning algorithms.

I am extracting and visualizing several audio features. This is done using the audio library librosa to extract frequency domain features (Mel-frequency Cepstral Coefficients (MFCC), Spectral Centroid, Spectral Roll-off...) and time domain features (Central moments, Zero Crossing Rate (ZCR), Root Means Squared Energy (RMSE)...). Those are then fed into one or several classifiers for comparison (logistic regression, random forest, gradient boosting, support vector machines...). 

For now, the dataframe being used is the one provided by the GTZAN dataset on Kaggle. For a future implementation, the idea is to generate a dataframe from the dataset itself. Also to experiment with different (more robust) datasets,  deep learning models and deploy into a web application.