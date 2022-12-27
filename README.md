# MusicGenreClassifier_MiniProject

A music genre classifier using classic machine learning algorithms.

For the ML implementation, I would have to manually extract the features. This would be done using the audio library librosa to extract frequency domain features (Mel-frequency Cepstral Coefficients (MFCC), Spectral Centroid, Spectral Roll-off...) and time domain features (Central moments, Zero Crossing Rate (ZCR), Root Means Squared Energy (RMSE)...). Those would then be fed into one or several classifiers for comparison (logistic regression, random forest, gradient boosting, support vector machines...).