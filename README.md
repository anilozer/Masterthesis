# Master Thesis – NLP – Topic Modeling

## A Comparison of Traditional vs. State-of-the-Art Methods

This repository contains the code and notebooks developed and used for my Master's thesis, which explores topic modeling in Natural Language Processing (NLP) by comparing a traditional statistical model (Latent Dirichlet Allocation – LDA) with a neural network-based model called [BERTopic](https://maartengr.github.io/BERTopic/index.html).

##  Thesis Abstract

Topic modeling aims to enhance human understanding and decision-making in complex textual datasets by clustering words and documents into meaningful groups. Traditional methods like LDA treat words statistically, while modern approaches such as BERTopic incorporate neural networks to capture semantic relationships.

This thesis undertakes a systematic comparison between LDA and BERTopic in terms of model effectiveness and human interpretability. A human evaluation survey was conducted where participants completed tasks such as generating titles, evaluating topic difficulty, and assessing keyword coherence.

The results demonstrate that neural topic models improve both topic coherence and diversity. However, a trade-off exists between maximizing topic diversity and maintaining interpretability. The study further reveals a notable alignment between machine-generated topics and human interpretation, particularly in thematic clustering, title generation, and keyword congruence.

##  Evaluation: Topic Diversity Metrics

To evaluate topic diversity, I implemented several metrics:

diversity_metrics.py, rbo.py, and word_embeddings_rbo.py were adapted from [silviatti/topic-model-diversity](https://github.com/silviatti/topic-model-diversity).

In alignment with Terragni et al. (2021), I extended the evaluation by implementing a BERT-based word embedding RBO (Rank-Biased Overlap) test. While Terragni used fastText embeddings, I opted for BERT to better capture contextual similarity.

##  Repository Structure

lda_model.ipynb: Topic modeling with LDA

bertopic_model.ipynb: Topic modeling with BERTopic

diversity_metrics.py: Implementation of topic diversity metrics

word_embeddings_rbo.py: BERT-based embedding similarity for topic comparison

rbo.py: Rank-Biased Overlap metric

survey_analysis.ipynb: Evaluation of human responses and survey analysis

## References
Terragni, S., et al. (2021). Topic Model Evaluation for User-Centered Tasks: A Case Study on Classification and Clustering.

[silviatti/topic-model-diversity](https://github.com/silviatti/topic-model-diversity)




