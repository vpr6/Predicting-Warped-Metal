# Predicting-Warped-Metal
Predicting Warped Metal

Turn Up (flattening) Prediction Model

This model uses turn-up data defined by amount of time to flatten a given piece.

Input data is the oncoming dimensions to the mill, the target final dimensions, abd the material type (Grade).

Original training showed that turn-up data was too small and so the model assumed that turn-up never happens.

To force the model to make a prediction of when turn up occurs (even if it causes more false positives), the data showing turn up was augmented with copies of pieces that turned up with random noise added in.

Final training showed 89.66% accuracy on training dataset, 80.92% accuracy on the test dataset, and 87.91% accuracy on the (non-agumented) original dataset.
