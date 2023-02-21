---
layout: page
title: faq
---

## FAQs

### 1. When the test data will be available?
The evaluation phase will start on **January, 2023**. Test data will be made available in **Codalab** prior the start period. 


### 2. How can I participate in the test phase?
A new Codalab submission site will be available before the evaluation phase. We will notify every participants from the practice phase with the link to the submission site for the test phase. Test predictions should be submitted to that site. For each track **maximum 6 submissions are allowed**. The **best result** will be used.


### 3. How large will be the test data?
The test data for each language will have at least 150K+ instances and for some languages there are approximately 500K+ instances. **As a result, generating predictions can take longer**.


### 4. How the final ranking will be determined? Will it consider per-domain F1?
Per-domain F1 will be shown in output JSON file, but final ranking will be determined based on overall macro-F1. However, the evaluation result will always display detailed result for each coarse and fine-grained classes.


### 5. Will I be able to see my results and the leaderboard during the test phase?
You can see the results on your submissions, but the leaderboard will not be available until after the competition.


### 6. Can we use an ensemble-based approach?
Yes, you can use any model for the task.


### 7. What are the domains of the test data?
The test data domains are similar as the development data. Looking at the development set will give an idea on the domains.

<!--

### 8. How much of the test entities overlap with the training entities?
This table provides the percentage of test data entities that are also found in the training sets.

<table style="width:60%">
  <tr>
    <th></th>
    <th>LOC</th>
    <th>PER</th>
    <th>PROD</th>
    <th>GRP</th>
    <th>CORP</th>
    <th>CW</th>
  </tr>


  <tr>
    <td>BN - Bangla</td>    
    <td>3.99</td>
    <td>1.54</td>
    <td>34.66</td>
    <td>7.15</td>
    <td>23.85</td>
    <td>4.33</td>
  </tr>
  
  <tr>
    <td>DE - German</td>
    <td>3.28</td>
    <td>2.76</td>
    <td>6.54</td>
    <td>5.68</td>
    <td>6.18</td>
    <td>3.7</td>
  </tr>
  
  <tr>
    <td>EN - English</td>
    <td>0.23</td>
    <td>0.15</td>
    <td>0.56</td>
    <td>0.38</td>
    <td>0.51</td>
    <td>0.2</td>
  </tr>
  
  <tr>
    <td>ES - Spanish</td>
    <td>0.39</td>
    <td>0.22</td>
    <td>0.58</td>
    <td>0.38</td>
    <td>0.55</td>
    <td>0.26</td>
  </tr>
  
  
  <tr>
    <td>FA - Farsi</td>
    <td>3.28</td>
    <td>4.39</td>
    <td>8.62</td>
    <td>9.83</td>
    <td>12.06</td>
    <td>5.9</td>
  </tr>
  
  <tr>
    <td>HI - Hindi</td>
    <td>4.84</td>
    <td>1.87</td>
    <td>30.33</td>
    <td>14.78</td>
    <td>21.24</td>
    <td>4.87</td>
  </tr>
  
  
    
  <tr>
    <td>KO - Korean</td>
    <td>5.73</td>
    <td>5.49</td>
    <td>12.32</td>
    <td>8.51</td>
    <td>11.24</td>
    <td>7.2</td>
  </tr>
  
  
  
  <tr>
    <td>NL - Dutch</td>
    <td>3.75</td>
    <td>3.7</td>
    <td>6.61</td>
    <td>5.12</td>
    <td>6.02</td>
    <td>4.53</td>
  </tr>
  
   <tr>
    <td>RU - Russian</td>
    <td>3.15</td>
    <td>1.36</td>
    <td>5.65</td>
    <td>3.91</td>
    <td>5.63</td>
    <td>3.82</td>
  </tr>
  
  <tr>
    <td>TR - Turkish</td>
    <td>0.61</td>
    <td>0.34</td>
    <td>1.72</td>
    <td>0.83</td>
    <td>1.64</td>
    <td>0.59</td>
  </tr>
  
  <tr>
    <td>ZH - Chinese</td>
    <td>4.28</td>
    <td>1.58</td>
    <td>15.38</td>
    <td>1.38</td>
    <td>7.65</td>
    <td>5.35</td>
  </tr>
  
</table>


### 9. How is the label distribution in the test data?
The plot below shows the label distribution in the train and test data. Y axis indicates the percentage of a particular label in the data.

<img src="images/dist.png">

### 10. How many unique entities are there?
This plot shows the total number of unique entities in the train and test sets.
<img src="images/unique_entities.png">

### 11. Since the test set is large, is there a way to efficiently output token tags for models using subword tokenizers?
We have implemented a method for doing this step. More details available <a href="https://github.com/amzn/multiconer-baseline/blob/main/README.md#:~:text=For%20this%20functionality">here</a>.

-->



