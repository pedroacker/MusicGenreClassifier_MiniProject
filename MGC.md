## Music Genre Classification using CNN or classic ML

For this project, I intend to deploy a music genre classifier into a web application. Music genre classification (MGC) has been a problem in music information retrieval (MIR) for a long time - starting with the problem of what a genre actually is. For this project, however, I assume that genre boundaries are somewhat known, and use a labeled dataset (GTZAN, Free Music Archive (FMA) or Audio set) to perform classification using either CNN or classic ML techniques, depending on time constraints. 

For the CNN implementation, transfer learning can be done using the VGG-16 architecture with the fixed weights, or just as a starting point. The NN consists of 5 convolutional blocks, and the output layer would be a softmax activation. I would need to download the architecture, change the output layer, use regularization and dropout to reduce overfitting (reported by the referencee) and feed the songs' spectrograms as inputs. 

For the ML implementation, I would have to manually extract the features. This would be done using the audio library librosa to extract frequency domain features (Mel-frequency Cepstral Coefficients (MFCC), Spectral Centroid, Spectral Roll-off...) and time domain features (Central moments, Zero Crossing Rate (ZCR), Root Means Squared Energy (RMSE)...). Those would then be fed into one or several classifiers for comparison (logistic regression, random forest, gradient boosting, support vector machines...).

The evaluation consists of standard accuracy, f-score and AUC scores.

Future related ideas could be speech classification or noise reduction, but both of those seem considerably more complex and less flexible (solely based on DL with RNN, LSTM and CNN with millions of parameters and extensive literature background).

Main reference:
Bahuleyan, Hareesh. Music Genre Classification using Machine Learning Techniques. University of Waterloo, 2018.