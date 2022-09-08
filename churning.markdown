---
layout: page
title: churning
permalink: /churning/
---
My guide to credit card churning.

### theory
Most people can be categorized into one of the following levels based on the mechanism through which they spend money.

**Level 0:** Only using cash/debit card. This is significantly worse than using a credit card, as you lose many of the valuable benefits of using a credit card (building credit, fraud protection, etc.). However, it's plausible that this is the optimal point for those who struggle with keeping track of finances/remembering to make payments/spending responsibly.

**Level 1:** Only using a single credit card, usually one with no annual fee and very little cashback (1-1.5%), likely issued by the individual's primary bank. This is much better than not having a credit card, but far from optimal, due to the low cashback/lack of benefits on the credit card. Most people fall into this category.

**Level 2:** Only using a single credit card, but one that was chosen with some amount of thought. Maybe this card has no annual fee but comparatively high cashback (2-2.5%), or maybe the card has an annual fee but comes with high cashback in useful categories (dining, travel) and other nice perks (travel insurance, lounge access, travel/food credits). This is an improvement over level 1, but not a large one.

**Level 3 (?):** Using multiple category-based cashback credit cards. This is theoretically better than level 2 (e.g. it's possible to craft some portfolio of credit cards such that you're able to get ~5% back on the majority of expenses) but I personally find it less optimal, since every time you make a purchase you have to think about which of your 10 credit cards you should use (also, you have to bring all your cards with you everywhere, for the places that don't take Apple Pay).

**Level 4:** Continuously applying for new cards to collect their signup bonuses after meeting the minimum spend requirement. The return on capital here is extremely high (e.g. >10% back). There is some startup cost here, since banks have rules in place to prevent inidividuals from egregiously taking advantage of these signup bonuses, and it's important to understand these rules when starting out. There is also some work involved with keeping track of bonuses/annual fees, filling out credit card applications, etc. but it's not large as long as you're reasonably organized.

**Level 5:** This is level 4, but fully optimized using a variety of strategies. Most individuals in this level are limited in their returns not by the amount of money they are able to "spend", but by the amount of cards that banks will let them apply for. 

This writeup focuses on level 4/5.

### glossary

| term | definition |
| --- | --- |
| SUB | signup bonus |
| MSR | minimum spend requirement (for signup bonus) |

### quickstart
In general, you can only receive a SUB for a card every 24 months (with some exceptions), and so you should try to apply for cards when the signup bonus is at an all-time high. You shouldn't apply for cards too frequently (e.g. multiple cards in a week), since frequent hard pulls will negatively impact your credit score. Some banks have velocity limits on how often you can apply for their cards (e.g. applying for a Chase card more than once every 3 months will put you at risk of shutdown). 

By far the most restrictive anti-churning rule is Chase's 5/24 rule: you can only be approved for a Chase card if you have been approved for less than 5 personal cards (from any issuer) in the past 24 months. As a result, it is generally recommended to apply for Chase cards first, and then apply for non-Chase cards after exceeding 5/24. (This is less relevant for those who plan to never exceed 5/24, e.g. by mostly applying for business cards).

Business cards are also a valuable source of return - they generally have higher MSRs but also come with high SUBs. Some have fewer restrictions on how often you can receive the SUB (e.g. Chase business cards have no such restriction). Most importantly, they generally don't count towards 5/24.

The optimal credit card application path varies from person to person and depends on factors such as credit score, amount of spending, airline/hotel preferences, etc. (For example, an individual living in New York would probably not get much value out of Southwest cards, but someone living in California might.)

The two primary card issuers are Chase and Amex, and most strategies revolve around their cards. Other card issuers of interest, in very approximate order of importance, include Barclays, Capital One, Citibank, US Bank, and Bank of America.

### resources
[r/churning](https://reddit.com/r/churning): The primary repository of churning knowledge. The daily question/discussion threads are great places to learn and ask questions, and the wiki is also useful (although a bit outdated).
* 

### breakdown by bank
{% for bank in site.banks %}
  <h3>{{ bank.name }}</h3>
  <p>{{ bank.content | markdownify }}</p>
{% endfor %}