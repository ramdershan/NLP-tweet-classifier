# NLP-tweet-classifier

This project involves training a text classifier that classifies tweets as either a natural disaster or not a natural disaster. For example, if someone tweets "That's fire :fire:", is it actually a fire (natural disaster) or is it an exaggeration (not natural disaster). The dataset used can be found in this repo but I got it from kaggle's Natural Language Processing (NLP) with Disaster Tweets competition. My most recent model achieved an F1 score of 0.81581 on unseen data when submitted to kaggle and is ranked at 185. 

## Files

<ul>
  <li>data</li>
    <ul>
      <li>sample_submission.csv</li>
      <li>test.csv</li>
      <li>train.csv</li>
    </ul>
  <li>nlptweetshuggingfacetransformer.ipynb</li>
  <li>nlptweetstf.ipynb</li>
</ul>

## Details

**nlptweetstf.ipynb** contains a basic RNN using LSTMs and was based on a tensorflow tutorial I did to learn and understand the processes required to train a NLP model.

**nlptweetshuggingfacetransformer.ipynb** contains my most recent model. I used the Hugging Face library to fine-tune a transformer model to classify the tweets. I imported *bertweet-base* from *vinai* and fine-tuned it on my dataset for my task.
