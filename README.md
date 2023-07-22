# amazon-multiinput-sentiment-classification-with-bert
Amazon MultiInput Sentiment Classification with BERT

# Introduction

We've been doing text classification 📖 with just **one input** for every target, be it [binary](https://www.kaggle.com/code/wesleyacheng/movie-review-sentiment-classifier-with-bert) or [multiclass](https://www.kaggle.com/code/wesleyacheng/news-topic-classification-with-bert) or [multilabel](https://www.kaggle.com/code/wesleyacheng/hate-speech-multilabel-classification-with-bert). The fun thing about most real-world 🌎 problems are that they usually have **multiple inputs**. 

<img width="491" alt="amazon-reviews" src="https://github.com/wesleyacheng/amazon-multiinput-sentiment-classification-with-bert/assets/15952538/cb4727c4-a39e-4213-8e78-a30b485d460c">

For example, in order to **classify a Amazon product review** 📦, we can not only use the **review content**, but we can include the **review title** as well. Having **multiple inputs** allows the model to **better understand the context** in which it is used, while usually **increasing or having similar performance** to that of a single input 😮. One can also add **too many inputs** model that may cause a **substantial reduction** in performance, especially if the truncation of each input context is **severe** like reducing a sentence the first word 😢. **But in general, combining/concatenating inputs are a useful deep learning 🤖  technique to have in your arsenal 🛡.**

In this notebook, we will be, as hinted above 🙃, classifying product review sentiment using both the review title **AND** content! 😁

**Results TLDR:** Review Title + Review Content > Review Content > Review Title
