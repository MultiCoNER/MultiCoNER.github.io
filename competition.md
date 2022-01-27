---
layout: page
title: "Competition"
permalink: /competition
order : 1
---

## 1. How to Participate
* The organizers have defined a task (i.e., NER) and released the training data on September 3rd. The task is divided across several languages as subtasks. The participants can work on as many as languages they want to.
* Participants can form a team with multiple people or single person team is okay.
* The participants can access the training data after filling the form in the <a href="/dataset" target="_blank">Dataset</a> page. 
* The participants can experiment with the training data to develop models. Usage of any external data or resource is allowed and highly encouraged. This process can run till the evaluation period.
* __Evaluation period__: On January 24th, the organizers will release the test set containing instances without the labels. The participants will use their developed models to predict the labels for the instances and they have to create a submission file that follows exactly the same format of the training data. These prediction files should be submitted to Codalab submission portal (will be announced later). These predictions will be compared against the ground truth labels of the test data and the teams will be ranked on a leaderboard according to the performance score.
* Each team is encouraged to write a system description paper describing their submission system, analysis of their results, interesting insights and submit before around February 23rd, 2022. Paper submission procedure will be announced later. After a review period, each team has to update their submitted paper based on the review feedback and submit the camera ready version. Accepted papers will be published as part of the proceedings of <a href="https://semeval.github.io" target="_blank">SemEval 2022 Workshop</a>.
* To connect with the organizers or other participants about any questions or discussions, participants can join the <a href="https://join.slack.com/t/multiconer/shared_invite/zt-vi3g97cx-MpqTvS07XX22S78nRC2s0Q" target="_blank">Slack</a> and Google group.



## 2. Training Data Format
<a href="data/semeval_2021_task_11_trial_data.txt" download>Click here to download a small set of trial data in English.</a>

We will follow the [CoNLL](https://universaldependencies.org/docs/format.html) format for the datasets. Here is an example data sample from the trial data.

![.](images/trial_data_sample.png)


In a data file, samples are separated by blank lines. Each data instance is tokenized and each line contains a single token with the associated label in the last (4th) column. Second and third columns (`_`) are ignored. Entities are labeled using the [BIO](https://natural-language-understanding.fandom.com/wiki/Named_entity_recognition#BIO) scheme. That means, a token tagged as `O` is not part of an entity, `B-X` means the token is the first token of an `X` entity, `I-X` means the token is in the boundary (but not the first token) of an `X` type entity having multiple tokens. In the given example, the input text is:

> the original ferrari daytona replica driven by don johnson in miami vice

The following image shows the entities as annotated.
![.](images/trial_sample_viz.png)

Here are some examples from the other languages.
* <span style="color:#274277"><b>Bangla:</b></span> ![.](images/b/BN.png)
* <span style="color:#274277"><b>Chinese:</b></span>![.](images/b/ZH.png)
* <span style="color:#274277"><b>Hindi:</b></span>![.](images/b/HI.png)
* <span style="color:#274277"><b>Korean:</b></span>![.](images/b/KO.png)
* <span style="color:#274277"><b>German:</b></span> ![.](images/b/DE.png)
* <span style="color:#274277"><b>Russian:</b></span>![.](images/b/RU.png)
* <span style="color:#274277"><b>Turkish:</b></span>![.](images/b/TR.png)
* <span style="color:#274277"><b>Farsi:</b></span>![.](images/b/FA.png)
* <span style="color:#274277"><b>Dutch:</b></span>![.](images/b/NL.png)
* <span style="color:#274277"><b>Spanish:</b></span> ![.](images/b/ES.png)





<!--## Official Competition Metric for the Task-->


## 3. Label Space
In this task, we focus on the following six entity types:
1. __PER__ : Person
2. __LOC__ : Location
3. __GRP__ : Group
4. __CORP__ : Corporation
5. __PROD__ : Product
6. __CW__: Creative Work


## 4. Evaluation 
In this shared task, we provide train/dev/test data for 11 languages. Additionally, we provide dev and test sets for <a href="https://en.wikipedia.org/wiki/Code-mixing" target="_blank">code-mixed language</a> (Find relevant resources in Section 6). As a summary, we provide 11 training files and 12 dev/test files. This codalab competition is in practice phase, where you are allowed to submit prediction file for dev sets. The evaluation framework is divided in three broad tracks. 
1. **Multi-lingual (Track 1)**: In this track, the participants have to train a single multi-lingual NER model using training data for all the languages. This model should be used to generate prediction files for each of the 11 languages’ evaluation (dev/test) set and a code-mixed evaluation set. That means the model should be able to handle monolingual data from any of the languages and code-mixed cases as well.\\
<span style="color:red">Predictions from any **mono-lingual** model is not allowed in this track. Therefore, please do not submit predictions from mono-lingual models in this track.</span>.

2. **Mono-lingual (Tack 2-12)**: In this track, the participants have to train a model that works for only one language. For each language, there will be one dev/test set that contains examples for that particular language. Participants have to train a mono-lingual model for the language of their interest and use that to create prediction file for the evaluation set of that language.\\
<span style="color:red">Predictions from any **multi-lingual** model is not allowed in this track.</span>

3. **Code-mixed (Tack 13)**: This test data contains have code-mixed samples. These samples will include tokens from any of the 11 mentioned languages in the shared task. This is an additional test set apart from the 11 mono-lingual test sets.

## 5. Submission Instructions
The evaluation script is based on [conlleval.pl](https://github.com/chakki-works/seqeval/blob/master/tests/conlleval.pl). 
### 5.1. Format of prediction file
The prediction file should follow [CoNLL](https://universaldependencies.org/format.html) format but only contain tags. That means, each line contains only the predicted tags of the tokens and sentences are separated by a blank line. Make sure your tags in your prediction file are exactly aligned with the provide dev/test sets.  For example, 
* Given `en_dev.conll` or `en_test.conll`
    * 
        ```
      # id f423a88e-02b7-4d61-a546-4a1bd89cfa15    domain=dev
        it _ _ _
        originally _ _ _
        operated _ _ _
        seven _ _ _
        bus _ _ _
        routes _ _ _
        which _ _ _
        were _ _ _
        mainly _ _ _
        supermarket _ _ _
        routes _ _ _
        for _ _ _
        asda _ _ _
        and _ _ _
        tesco _ _ _
        . _ _ _
        
        ...
      ```
        
* You will need generate the prediction file `en.pred.conll` in the follow format
    * 
        ```
        #(You can either delete sentence id or keep it)
        O
        O
        O
        O
        O
        O
        O
        O
        O
        O
        O
        O
        B-CORP
        O
        B-CORP
        O
        
        ...
        ```
        
### 5.2. Prepare submission files
Follow the below instructions to submit your prediction files for a track. Codalab requires all submissions in zip format

* Use your trained model to generate a prediction file for a specific tack and name it in this format: `<language_code>.pred.conll`. 
    * For example, when you participate in the English track, you will need to generate a prediction file for en_dev.conll (or en_test.conll in the testing phase) and name it as en.pred.conll.
    * The language_code values for  **Track 12 Multilingual** and **Track 13 code mixed** are **multi** and **mix**, respectively. That means, you will need to name the prediction file as `multi.pred.conll` or `mix.pred.conll`.
* Compress the `<language_code>.pred.conll` file to a zip file by using zip `my_submission.zip <language_code>.pred.conll` (or your favorite zip utility), and the submit the zip file to the right track on Codalab.




## 6. Some Resources for the Beginners in NLP
* <a href="https://en.wikipedia.org/wiki/Named-entity_recognition" target="_blank">Wikipedia article on Named Entity Recognition</a>
* <a href="https://www.youtube.com/watch?v=MY9fs1Plh_o" target="_blank">Lecture from Prof. Chris Manning on the Evaluation of Named Entity Recognition</a>
* <a href="https://www.geeksforgeeks.org/python-named-entity-recognition-ner-using-spacy" target="_blank">Named Entity Recognition (NER) using spaCy in Python</a>
* <a href="https://medium.com/analytics-vidhya/custom-named-entity-recognition-ner-model-with-spacy-3-in-four-steps-7e903688d51" target="_blank">Custom Named Entity Recognition (NER) model with spaCy 3 in Four Steps</a>
* <a href="https://keras.io/examples/nlp/ner_transformers" target="_blank">Named Entity Recognition using Transformers with Keras</a>
* <a href="https://cs230.stanford.edu/blog/namedentity" target="_blank">Named Entity Recognition Tagging with Pytorch</a>
* <a href="https://skimai.com/how-to-fine-tune-bert-for-named-entity-recognition-ner/" target="_blank">How to Fine tune BERT for NER</a>
* <a href="http://nlpprogress.com/english/named_entity_recognition.html" target="_blank">Recent SOTA Papers for NER systems in NLP Progress</a>
* <a href="https://ritual.uh.edu/lince/home">Code Switching Leaderboard LinCE.</a>
* <a href="https://aclanthology.org/W18-3219.pdf">Named Entity Recognition on Code-Switched Data:
Overview of the CALCS 2018 Shared Task</a>

### Communication
* Join us in <a href="https://join.slack.com/t/multiconer/shared_invite/zt-vi3g97cx-MpqTvS07XX22S78nRC2s0Q" target="_blank">Slack</a>

* Subscribe to the [task mailing list](mailto:multiconer-semeval@googlegroups.com)

* [Contact the organizers](mailto:multiconer-semeval-organizers@googlegroups.com)