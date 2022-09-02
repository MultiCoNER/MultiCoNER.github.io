---
layout: page
title: "Complex Named Entity Recognition Across Languages"
permalink: 
order: 1
---
<br/><br/>

Complex  named  entities  (NE),  like  the  titles  of creative works, are not simple nouns and pose challenges for NER systems (Ashwini and Choi, 2014). They can take the form of any linguistic constituent, like  an  imperative  clause  (“Dial M for Murder”), and do not look like traditional NEs (Persons, Locations, etc.).  This syntactic ambiguity makes it challenging to recognize them based on context. We organized the <a href="https://aclanthology.org/2022.semeval-1.196.pdf" target="_blank">MultiCoNER task (Malmasi et al., 2022)</a> at SemEval-2022 to address these challenges in 11 languages, receiving a very positive community response with 34 system papers. Results confirmed the challenges of processing complex and long-tail NEs: even the largest pre-trained Transformers did not achieve top performance without external knowledge. The top systems infused transformers with knowledge bases and gazetteers. However, such solutions are brittle against out of knowledge-base entities and noisy scenarios like the presence of spelling mistakes and typos. We  propose MultiCoNER II which  represents novel challenges through new tasks that emphasize the shortcomings of the current top models. 

MultiCoNER II features complex NER in these languages:

<ol>
<li> English </li>
<li> Spanish </li>
<li> Hindi </li>
<li> Bangla </li>
<li> Chinese </li>
<li> Swedish </li>
<li> Farsi </li>
<li> French </li>
<li> Italian </li>
<li> Portugese </li>
<li> Ukranian </li>
<li> German </li>
</ol>


### MultiCoNER I: SemEval 2022 Task 11
* <a href="https://aclanthology.org/2022.semeval-1.196.pdf" target="_blank">Task overview paper </a>
* <a href="https://assets.amazon.science/1a/b3/e091bdd94d0f9e5d2963e2dd6943/multiconer-a-large-scale-multilingual-dataset-for-complex-named-entity-recognition.pdf" target="_blank"> Dataset Paper</a>
* <a href="https://multiconer.github.io/multiconer_1/" target="_blank">Website</a>
* <a href="https://competitions.codalab.org/competitions/36044" target="_blank">Codalab</a>
* <a href="https://multiconer.github.io/multiconer_1/results" target="_blank">Ranking</a>


## References
* Sandeep Ashwini and Jinho D. Choi. 2014. [Targetable named entity recognition in social media](https://arxiv.org/pdf/1408.0782.pdf). _CoRR, abs/1408.0782_.
* Shervin Malmasi, Anjie Fang, Besnik Fetahu, Sudipta Kar, Oleg Rokhlenko. 2022. [SemEval-2022 Task 11: Multilingual Complex Named Entity Recognition (MultiCoNER)](https://aclanthology.org/2022.semeval-1.196.pdf).

<!--
* Jacob Devlin, Ming-Wei Chang, Kenton Lee, and Kristina Toutanova. 2019. [BERT: pre-training of deep bidirectional transformers for language understanding](https://aclanthology.org/N19-1423.pdf). _In NAACL-HLT (1). Association for Computational Linguistics_.
* Isabelle Augenstein, Leon Derczynski, and Kalina Bontcheva. 2017. [Generalisation in named entity recognition: A quantitative analysis](https://arxiv.org/pdf/1701.02877.pdf). _Computer Speech & Language, 44:61–83_.
* Jackson Luken, Nanjiang Jiang, and Marie-Catherine de Marneffe. 2018. [QED: A fact verification system for the FEVER shared task](https://aclanthology.org/W18-5526.pdf). _In Proceedings of the First Workshop on Fact Extraction and VERification (FEVER), pages 156–160, Brussels, Belgium. Association for Computational Linguistics_.
* Andreas Hanselowski, Hao Zhang, Zile Li, Daniil Sorokin, Benjamin Schiller, Claudia Schulz, and Iryna Gurevych. 2018. [UKP-athene: Multi-sentence textual entailment for claim verification](https://aclanthology.org/W18-5516.pdf). _In Proceedings of the First Workshop on Fact Extraction and VERification (FEVER), pages 103–108, Brussels, Belgium. Association for Computational Linguistics_.
-->



### Communication
* Join us in <a href="https://join.slack.com/t/multiconer/shared_invite/zt-vi3g97cx-MpqTvS07XX22S78nRC2s0Q">Slack</a>

* Subscribe to the [task mailing list](mailto:multiconer-semeval@googlegroups.com)

* [Contact the organizers](mailto:multiconer-semeval-organizers@googlegroups.com)


## Anti-Harassment Policy
SemEval highly values the open exchange of ideas, freedom of thought and expression, and respectful scientific debate. We support and uphold the [NAACL Anti-Harassment policy](http://naacl.org/policies/anti-harassment.html){:target="_blank"}. Participants are encouraged to send any concerns or questions to the [NAACL Board members](http://naacl.org/officers/){:target="_blank"}, [Priscilla Rasmussen](mailto://acl@aclweb.org){:target="_blank"} and/or the [workshop organizers](https://semeval.github.io/SemEval2022/){:target="_blank"}.
{: style="text-align: justify"}



