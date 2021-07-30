---
layout: page
title: "Complex Named Entity Recognition Across Languages"
permalink: /
order: 1
---


## Welcome

Processing complex and ambiguous Named Entities (NEs) is a challenging NLP task in practical and open-domain settings, but has not received sufficient attention from the research community.
{: style="text-align: justify"}

Complex NEs, like the titles of creative works (movie/book/song/software names) are not simple nouns and are harder to recognize (Ashwini and Choi, 2014). They can take the form of any linguistic constituent, like an imperative clause (“Dial M for Murder”), and do not look like traditional NEs (Person names, locations, organizations). This syntactic ambiguity makes it challenging to recognize them based on their context. Such titles can also be semantically ambiguous, e.g., “On the Beach” can be a preposition or refer to a movie. Finally, such entities usually grow at a faster rate than traditional categories, and emerging entities pose yet another challenge. Table 1 lists more details about these challenges, and how they can be evaluated.
{: style="text-align: justify"}

Neural models (e.g., Transformers) have produced high scores on benchmark datasets like CoNLL03/OntoNotes (Devlin et al., 2019). However, as noted by Augenstein et al. (2017), these scores are driven by the use of well-formed news text, the presence of “easy” entities (person names), and memorization due to entity overlap between train/test sets; these models perform significantly worse on complex/unseen entities. Researchers using NER on downstream tasks have noted that a significant proportion of their errors are due to NER systems failing to recognize complex entities (Luken et al., 2018; Hanselowski et al., 2018).
{: style="text-align: justify"}

![Examples of Complex Entities](images/table_1.png)



## References
* Sandeep Ashwini and Jinho D. Choi. 2014. [Targetable named entity recognition in social media](https://arxiv.org/pdf/1408.0782.pdf). _CoRR, abs/1408.0782_.
* Jacob Devlin, Ming-Wei Chang, Kenton Lee, and Kristina Toutanova. 2019. [BERT: pre-training of deep bidirectional transformers for language understanding](https://aclanthology.org/N19-1423.pdf). _In NAACL-HLT (1). Association for Computational Linguistics_.
* Isabelle Augenstein, Leon Derczynski, and Kalina Bontcheva. 2017. [Generalisation in named entity recognition: A quantitative analysis](https://arxiv.org/pdf/1701.02877.pdf). _Computer Speech & Language, 44:61–83_.
* Jackson Luken, Nanjiang Jiang, and Marie-Catherine de Marneffe. 2018. [QED: A fact verification system for the FEVER shared task](https://aclanthology.org/W18-5526.pdf). _In Proceedings of the First Workshop on Fact Extraction and VERification (FEVER), pages 156–160, Brussels, Belgium. Association for Computational Linguistics_.
* Andreas Hanselowski, Hao Zhang, Zile Li, Daniil Sorokin, Benjamin Schiller, Claudia Schulz, and Iryna Gurevych. 2018. [UKP-athene: Multi-sentence textual entailment for claim verification](https://aclanthology.org/W18-5516.pdf). _In Proceedings of the First Workshop on Fact Extraction and VERification (FEVER), pages 103–108, Brussels, Belgium. Association for Computational Linguistics_.


## Anti-Harassment Policy
SemEval highly values the open exchange of ideas, freedom of thought and expression, and respectful scientific debate. We support and uphold the [NAACL Anti-Harassment policy](http://naacl.org/policies/anti-harassment.html){:target="_blank"}. Participants are encouraged to send any concerns or questions to the [NAACL Board members](http://naacl.org/officers/){:target="_blank"}, [Priscilla Rasmussen](acl@aclweb.org){:target="_blank"} and/or the [workshop organizers](https://semeval.github.io/SemEval2022/){:target="_blank"}.
{: style="text-align: justify"}

<!-- ## Sponsored By       
<!-- ![Computing Research Association’s Computing Community Consortium (CCC)](images/ccc_hz copy.jpg)
![National Science Foundation](images/NSF_4-Color_bitmap_Logo.png =250x)
 -->
<!-- <img src="images/ccc_hz copy.jpg" alt="Computing Research Association’s Computing Community Consortium (CCC)" width="300"/>
<img src="images/NSF_4-Color_bitmap_Logo.png" alt="National Science Foundation" width="200"/>
<img src="images/nrc_canada_logo.png" alt="National Research Council, Canada" width="250" style="padding: 0 0 0 40px"/>
<img src="images/google_logo.svg" alt="Google" width="250" style="padding: 0 0 0 40px"/> --> 



