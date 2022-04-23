# Sentiment-Classification

This is a code that I have written by following the sentiment classification module in Udacity. I used PyTorch framework for this project.

The model takes a review as an input and provides 0 or 1 as an output. The output **0** corresponds to a **negative** review and the output **1** corresponds to a **positive** review.

The model summary:
* Embedding layer: Embedding(74073, 500)
* LSTM layer: LSTM(500, 256, num_layers=2, batch_first=True, dropout=0.5)
* Fully Connected Layer: Linear(in_features=256, out_features=1, bias=True)

The model has been trained for 5 epochs using stochastic gradient descent algorithm. The testing accuracy and losses are as follows,
* Test Loss: 0.211
* Testing Accuracy: 92.5%

After the testing, 2 custom reviews are written to test the model, which produced expected results when tested.
