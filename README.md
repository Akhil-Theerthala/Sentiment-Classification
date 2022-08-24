# Sentiment-Classification


## Motivation:

**Github Link**: [Movie Review Sentiment Classification](https://github.com/Akhil-Theerthala/Sentiment-Classification)

The goal of the project is to identify the sentiment of a movie review. The model takes a review as an input and provides 0 or 1 as an output. The output **0** corresponds to a **negative** review and the output **1** corresponds to a **positive** review. 

---

## Model Architechture:
```
Sentiment_analysis(
  (embed): Embedding(74073, 500)
  (lstm): LSTM(500, 256, num_layers=2, batch_first=True, dropout=0.5)
  (fc): Linear(in_features=256, out_features=1, bias=True)
)
```

---

## Performance:
The model has been trained for 5 epochs using stochastic gradient descent algorithm. The testing accuracy and losses are as follows,
* Test Loss: 0.211
* Testing Accuracy: 92.5%

After the testing, 2 custom reviews are written to test the model, which produced expected results when tested.

* Postive review test:

Review: ***"What a wonderful experience this was! I was on the edge of my seat when I watched this movie. I still recall all the scenes. When I watched the intermission, I got goosebumps. I would definitely watch this movie again"***

![image](https://user-images.githubusercontent.com/85566221/186479948-9fe96bc0-fb7c-47b9-92e9-2a0ed335c0ee.png)

* Negative review test:

Review: ***" This is the worst movie that anyone could possibly make. I still cannot understand why the producer invested so much in this movie. The recently released low budget movie was better than this one. I probably would never watch this one again "***

![image](https://user-images.githubusercontent.com/85566221/186480009-6b1aa6fb-c07b-42f4-9516-76be2f6f148a.png)
