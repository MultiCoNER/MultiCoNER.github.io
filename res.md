---
layout: page
title: "Competition"
permalink: /competition
order : 1
---

## Competition

We will be using CodaLab for the competition. Details are coming soon.


## Data Format
<a href="data/semeval_2021_task_11_trial_data" download>Click here to download a small set of trial data in English.</a>

We will follow the [CoNLL](https://universaldependencies.org/docs/format.html) format for the datasets. Here is an example data sample from the trial data.

![.](images/trial_data_sample.png)


In a data file, samples are separated by blank lines. Each data instance is tokenized and each line contains a single token with the associated label in the last (4th) column. Second and third columns (`_`) are ignored. Entities are labeled using the [BIO](https://natural-language-understanding.fandom.com/wiki/Named_entity_recognition#BIO) scheme. In the given example, the input text is:

> the original **ferrari daytona** replica driven by **don johnson** in **miami vice**

The bold tokens are part of named entities. `ferrari daytona` is a `PRODUCT` entity, `don johnson` is a `PERSON` entity, and `miami vice` is a `CREATIVE WORK` entity.

<!--## Official Competition Metric for the Task-->
