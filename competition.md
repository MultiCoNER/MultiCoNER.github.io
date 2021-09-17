---
layout: page
title: "Competition"
permalink: /competition
order : 1
---

## How to Participate
* The organizers have defined a task (i.e., NER) and released the training data on September 3rd. The task is divided across several languages as subtasks. The participants can work on as many as languages they want to.
* Participants can form a team with multiple people or single person team is okay.
* The participants can access the training data after filling the form in the <a href="/dataset" target="_blank">Dataset</a> page. 
* The participants can experiment with the training data to develop models. Usage of any external data or resource is allowed and highly encouraged. This process can run till the evaluation period.
* __Evaluation period__: Around January 10th, the organizers will release the test set containing instances without the labels. The participants will use their developed models to predict the labels for the instances and they have to create a submission file that follows exactly the same format of the training data. These prediction files should be submitted to Codalab submission portal (will be announced later). These predictions will be compared against the ground truth labels of the test data and the teams will be ranked on a leaderboard according to the performance score.
* Each team is encouraged to write a system description paper describing their submission system, analysis of their results, interesting insights and submit before around February 23rd, 2022. Paper submission procedure will be announced later. After a review period, each team has to update their submitted paper based on the review feedback and submit the camera ready version. Accepted papers will be published as part of the proceedings of <a href="https://semeval.github.io" target="_blank">SemEval 2022 Workshop</a>.
* To connect with the organizers or other participants about any questions or discussions, participants can join the <a href="https://join.slack.com/t/multiconer/shared_invite/zt-vi3g97cx-MpqTvS07XX22S78nRC2s0Q" target="_blank">Slack</a> and Google group.



## Data Format
<a href="data/semeval_2021_task_11_trial_data.txt" download>Click here to download a small set of trial data in English.</a>

We will follow the [CoNLL](https://universaldependencies.org/docs/format.html) format for the datasets. Here is an example data sample from the trial data.

![.](images/trial_data_sample.png)


In a data file, samples are separated by blank lines. Each data instance is tokenized and each line contains a single token with the associated label in the last (4th) column. Second and third columns (`_`) are ignored. Entities are labeled using the [BIO](https://natural-language-understanding.fandom.com/wiki/Named_entity_recognition#BIO) scheme. That means, a token tagged as `O` is not part of an entity, `B-X` means the token is the first token of an `X` entity, `I-X` means the token is in the boundary (but not the first token) of an `X` type entity having multiple tokens. In the given example, the input text is:

> the original ferrari daytona replica driven by don johnson in miami vice

The following image shows the entities as annotated.
![.](images/trial_sample_viz.png)
<!--## Official Competition Metric for the Task-->


## Label Space
In this task, we focus on the following six entity types:
1. __PER__ : Person
2. __LOC__ : Location
3. __GRP__ : Group
4. __CORP__ : Corporation
5. __PROD__ : Product
6. __CW__: Creative Work


## Some Resources for the Beginners in NLP
* <a href="https://en.wikipedia.org/wiki/Named-entity_recognition" target="_blank">Wikipedia article on Named Entity Recognition</a>
* <a href="https://www.youtube.com/watch?v=MY9fs1Plh_o" target="_blank">Lecture from Prof. Chris Manning on the Evaluation of Named Entity Recognition</a>
* <a href="https://www.geeksforgeeks.org/python-named-entity-recognition-ner-using-spacy" target="_blank">Named Entity Recognition (NER) using spaCy in Python</a>
* <a href="https://medium.com/analytics-vidhya/custom-named-entity-recognition-ner-model-with-spacy-3-in-four-steps-7e903688d51" target="_blank">Custom Named Entity Recognition (NER) model with spaCy 3 in Four Steps</a>
* <a href="https://keras.io/examples/nlp/ner_transformers" target="_blank">Named Entity Recognition using Transformers with Keras</a>
* <a href="https://cs230.stanford.edu/blog/namedentity" target="_blank">Named Entity Recognition Tagging with Pytorch</a>
* <a href="https://skimai.com/how-to-fine-tune-bert-for-named-entity-recognition-ner/" target="_blank">How to Fine tune BERT for NER</a>
* <a href="http://nlpprogress.com/english/named_entity_recognition.html" target="_blank">Recent SOTA Papers for NER systems in NLP Progress</a>

### Communication
* Join us in <a href="https://join.slack.com/t/multiconer/shared_invite/zt-vi3g97cx-MpqTvS07XX22S78nRC2s0Q" target="_blank">Slack</a>

* Subscribe to the [task mailing list](mailto:multiconer-semeval@googlegroups.com)

* [Contact the organizers](mailto:multiconer-semeval-organizers@googlegroups.com)