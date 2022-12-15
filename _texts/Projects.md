---
layout: page
title: Projects
---
## Language Use Regarding Eating Disorders and Female Athletes


The question I had in mind when I began this project was:

*How are people who hold positions of authority within female athletics responding to and working to prevent eating disorders and disordered eating habits?*

I chose this question because previous research shows that 46% of elite female athletes involved in "leanness sports" (like gymnastics, cross country, or dancing) enagage in disordered eating behaviors or show signs of eating disorders[^fn1]. These behaviors are connected to injury, menstrual dysfunction, increased depressive tendencies, decreased athletic performances, hormonal imbalance, nutrient deficiencies, and a myriad of other risks[^fn2]. Knowing these statistics, I expected and hoped my research would demonstrate that authorities within female athletics would emphasize education about, identification of, and treatment of eating disorders.


#### Search Results

I analyzed 17 articles from <a href="https://meridian.allenpress.com/jat"><em>The Journal of Athletic Training</em></a> using a topic model to try and understand the language around eating disorders and disordered eating in female athletics. The *JAT* has 5,675 articles available in their online search. Searching the terms "eating disorder," "eating disorders," or "disordered eating," yields only 95 results, or about **0.01674%** of the journal's online corpus. Comparitvely earching for a specific injury, like "ankle sprain" or "muscle strain," yields 502 results (0.0885% of total) and 378 results (0.0667% of total), respectively. While muscle strains and ankle sprains are likely more common ailments among athletes, the small percentage of results for search terms related to eating pathology does not correlate with the amount of athletes who suffer from the disorders.

![Search Results](/ed/search-results.png)

#### Google NGrams

Google Ngrams reflects that the terms "eating disorder" began to sharply increase in use in 1980. While this data would likely be useful if I were to expand the corpus of this project, the *JAT* only has documents available online from 2008-the present.



#### Topic Modeling

Using [*Mallet*](https://mallet.cs.umass.edu/diagnostics.php), I made 19 topics of 25 terms each for my corpus. Unsurprisngly, "sports" was the term with the highest degree centrality. All terms with degree centality measure equal to or greater than 3 are listed below.

| 3           | 4         | 5          | 6        | 7      |
| ------------|-----------|------------|----------|--------|
| image       | sport     | collegiate | athlete  | sports |
| division    | risk      | health     | athletes |        |
| weight      | disorders |            | injury   |        |
| screening   | eating    |            |          |        |
| issues      | trainers  |            |          |        |
| group       | female    |            |          |        |
| athletic    |           |            |          |        |
| performance |           |            |          |        |
| ats         |           |            |          |        |
| energy      |           |            |          |        |
| low         |           |            |          |        |
| mass        |           |            |          |        |
| study       |           |            |          |        |
| bone        |           |            |          |        |
| injuries    |           |            |          |        |

Again, it was unsurprisng to find that "athlete," "athletes," and "collegiate" were among the terms that occured in the most topics. The presence of "injury," however, contributes to the idea that discussion regarding eating disorders and female athletes considers injuries a prevalent issue, and seeks to address this. Because of the tendency for bone injuries to co-occur with eating pathologies, it was comforting to see the frequency of "injury," "injuries," and "bone" in the topic model[^fn3].

The recurrence of "performace" was interesting as well, as eating pathologies are associated with decreased performance, indicating that the discussion around eating disorders and female athletes might consider the effect that eating pathologies can have on performance.

The terms "female" (4) and "women" (1) had lower degree centralities than I expected, potentially indicating that while the *JAT* acknowledges the effects of eating pathologies, they do not associate these habits with female athletes more than male athletes. "Prevention" (2) and "treatment" (2) also appeared in less topics than I anticipated, suggesting that the *JAT* literature might not focus on treatment and prevention of eating pathologies in their articles.

![Topic Model](/Users/HannahBallowe/ed/assets/topicmodel.png)

The topic model above does not show us anything substantial, because of the scale, but the magnified image below show us the number of edges connected to the term "sports" (in red), showing how many topics "sports" occurs in.

!["Sports" edges](/Users/HannahBallowe/ed/assets/sports.png)

Likewise, the image below shows the relatively smaller number of edges (in red) connected to the term "treatment," and the two topics it occurs in.

!["Treatment" edges](/Users/HannahBallowe/ed/assets/treatment.png)

Finally, the image below shows an example of one of the topics generated by *Mallet* and the terms included within that topic. Terms not shown in this image but present in the topic include "members," "eating," "female," "image."

![Topic 20](/Users/HannahBallowe/ed/assets/topic20.png)

The association of "ideal," "body," "image," "bmi," and "fat" within this topic might suggest that *JAT* texts analyzed draw a connection between body image and eating disorders. This is interesting considering how the "body image" and "eating disorder" peaked in use at similar times in Google NGrams. 

![Google NGrams - "body image" and "eating disorder"](/Users/HannahBallowe/ed/assets/ngrams-body-eating.png)

#### Next Steps

The next step for this project as a whole would be to expand the corpus of texts I analyzed. While the *JAT* served as a fine starting point for applying skills and testing research methods, the limited date range and specific audience limits the credibility and legitimacy of my results. Though my results do not suggest that the audience of the *JAT* (athletic trainers) prioritize eating disorders in female athletes to the extent necessary, these results may be skewed by my sample size.

The next step for my topic model is to turn my bimodal graph into a unimodal one. Doing so would allow me to see what terms co-occur within topics, rather than just what terms occur in multiple topics.


[^fn1]:Melin, A., Tornberg, A., Skouby, S., Faber, J., Ritz, C., Sjodin, A., & Sundgot-Borgen, J. (2014, February 21). The LEAF questionnaire: A screening tool for the identification of female athletes at risk for the female athlete triad—ProQuest. ProQuest. https://www-proquest- com.ezproxy.lib.vt.edu/docview/1779357930/fulltext- PDF/AEE25FE0B94C479DPQ/1?ac countid=14826
[^fn2]: Mountjoy, M., Sundgot-Borgen, J., Burke, L., Carter, S., Constantini, N., Lebrun, C., Meyer, N., Sherman, R., Steffen, K., Budgett, R., & Ljungqvist, A. (2014a). The IOC consensus statement: Beyond the Female Athlete Triad—Relative Energy Deficiency in Sport (RED-S). British Journal of Sports Medicine, 48(7), 491–497.
[^fn3]: Edama, M., Inaba, H., Hoshino, F., Natsui, S., Maruyama, S., & Omori, G. (2021). The relationship be- tween the female athlete triad and injury rates in collegiate female athletes. PeerJ, 9, e11092. https://doi.org/10.7717/peerj.11092
