---
layout: page
title: churning
permalink: /churning/
exclude: false
---
My guide to credit card churning.

[theory](theory) 

## quickstart
There are already many good resources available for learning the basics of churning, so this guide will mostly focus on advanced tips for each bank/card. However, for those who are starting out, here are some resources:

[r/churning](https://reddit.com/r/churning): The primary repository of churning knowledge. The daily question/discussion threads are great places to learn and ask questions, and the wiki is also useful (although a bit outdated).
* [cc recommendation flowchart](https://www.reddit.com/r/churning/comments/s07cfp/credit_card_recommendation_flowchart_jan2022/): General churning guide geared towards beginners. The path that the flowchart recommends is not necessarily optimal for everyone, but it gets reasonably close and is a great starting point.
* [list of anti-churning rules](https://www.reddit.com/r/churning/comments/819r08/list_of_antichurning_rules/): Understanding the different anti-churning rules for each bank is one of the most important aspects of the hobby.
* [glossary](https://www.reddit.com/r/churning/wiki/glossary/): The many abbreviations used may seem daunting when getting started, so referencing the glossary is helpful.
* [churning.io](https://churning.io/): Extremely useful tool for searching r/churning.

And some more advanced resources:
* [chase biz card approval guide](https://www.reddit.com/r/churning/comments/844m2m/step_by_step_guide_to_getting_approved_for_chase/)
* [chase biz card verification guide](https://www.reddit.com/r/churning/comments/6hclj4/i_survived_the_dreaded_chase_business/)
* [doc reconsideration lines](https://www.doctorofcredit.com/credit-cards/credit-card-reconsideration-line-telephone-numbers/)

<br> 

---

<br> 

{% for bank in site.banks %}
  <h2>{{ bank.name }}</h2>
  <p>{{ bank.content | markdownify }}</p>
  {% for card in site.cards %}
    {% if card.bank == bank.name %} 
      <h3>{{ card.name }}</h3>
      <p>{{ card.content | markdownify }}</p>
    {% endif %} 
  {% endfor %}
{% endfor %}