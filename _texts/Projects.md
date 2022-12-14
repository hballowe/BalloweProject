---
layout: page
title: Projects
---
## Language Use Regarding Eating Disorders and Female Athletes


The question I had in mind when I began this project was:

*How are people who hold positions of authority within female athletics responding to and working to prevent eating disorders and disordered eating habits?*

I chose this question because previous research shows that 46% of elite female athletes involved in "leanness sports" (like gymnastics, cross country, or dancing) enagage in disordered eating behaviors or show signs of eating disorders (Melin et al). These behaviors are connected to injury, menstrual dysfunction, increased depressive tendencies, decreased athletic performances, hormonal imbalance, nutrient deficiencies, and a myriad of other risks (Mountyjoy et al). Knowing these statistics, I expected and hoped my research would demonstrate that authorities within female athletics would emphasize education about, identification of, and treatment of eating disorders.


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

Again, it was unsurprisng to find that "athlete," "athletes," and "collegiate" were among the terms that occured in the most topics. The presence of "injury," however, contributes to the idea that discussion regarding eating disorders and female athletes considers injuries a prevalent issue, and seeks to address this. Because of the tendency for bone injuries to co-occur with eating pathologies, it was comforting to see the frequency of "injury," "injuries," and "bone" in the topic model (Edama et al.).

The recurrence of "performace" was interesting as well, as eating pathologies are associated with decreased performance, indicating that the discussion around eating disorders and female athletes might consider the effect that eating pathologies can have on performance.

**image**

The terms "female" (4) and "women" (1) had lower degree centralities than I expected, potentially indicating that while the *JAT* acknowledges the effects of eating pathologies, they do not associate these habits with female athletes more than male athletes. "Prevention" (2) and "treatment" (2) also appeared in less topics than I anticipated, suggesting that the *JAT* literature might not focus on treatment and prevention of eating pathologies in their articles.

#### Next Steps

The next step for this project as a whole would be to expand the corpus of texts I analyzed. While the *JAT* served as a fine starting point for applying skills and testing research methods, the limited date range and specific audience limits the credibility and legitimacy of my results. Though my results do not suggest that the audience of the *JAT* (athletic trainers) prioritize eating disorders in female athletes to the extent necessary, these results may be skewed by my sample size.
<p>The next step for my topic model is to turn my bimodal graph into a unimodal one. Doing so would allow me to see what terms co-occur within topics, rather than just what terms occur in multiple topics.
</p>
