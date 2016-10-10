+++
categories = ["data", "health"]
date = "2016-10-03T14:44:46-07:00"
hero = "/img/food.jpg"
tags = []
title = "BMI Around the World Pt.1"
description = "Taking a look through different lenses"
disqus = true
+++

Like many in the United States, I often heard the adage of the "starving kids in China".
Nowadays, this is no longer a phrase I hear often. It may be because I
am no longer a child. The fact that not much of China is as poor or starving anymore,
I think, also plays a role in this. After all China has amazingly [reduced its poverty
rate from 88% to just 6% in the past 3 decades]
(http://www.worldbank.org/en/country/china/overview#3).

Even starving children in Africa are now considered rare(they do suffer from malnutrition however).

>[Thanks to economic growth and smart policies, the extreme hunger and starvation
that once defined the continent(Africa) are now rare.]
(https://www.gatesnotes.com/Development/Why-Does-Hunger-Still-Exist-Africas-Table-Day-One)

We no longer need to think of starving children in other countries as a push
to finish our plates and we could probably benefit from putting our fork down
as well. Obesity is becoming a real issue in the United States as
[1 in 3 children ages 6 to 19 are overweight or obese]
(https://www.niddk.nih.gov/health-information/health-statistics/Pages/overweight-obesity-statistics.aspx),
with the rate for adults being twice that.

It sounds bad. It *is* bad. However in relation to the rest of the world, it
shouldn't be come as a shock and we are not unique as indicated by an article
published by The Atlantic.

>[One-Third of the Global Population Is Overweight or Obese]
(http://www.theatlantic.com/international/archive/2014/05/one-third-of-the-world-is-obese-overweight/371790/)

With all of this in mind I wanted to get a visual representation of this.

## Results by region

As a quick reference the BMI classifications are:

Classification  |    Range   |   Color
--------------- | ---------- | -----------
Underweight     |  < 18.5    |  dark purple-purple
Normal weight   |  18.5–24.9 |  blue-green
Overweight      |  25–29.9   |  orange-red
Obesity         |  > 30      |  red-black


I used BMI data published by the WHO, and regional and income classifications
published by the World Bank to generate the graphs. The graphs use a colored
scale to indicate in what BMI range each country falls into.

As a note the WHO provides their own regional classifications for countries,
but I decided to not use it as I personally found it confusing and suspected it
would be for others as well. For example countries labelled as being in the
WHO's *South-East Asia* region include *Maldives, Bhutan, Sri Lanka, Nepal, India, Bangladesh, and North Korea*.

Using the World Bank's regional grouping:

{{<highchartsTreeBMI src="/charts/bmi.json" metasrc="/charts/worldbank2014m.json" id="bmi-wb-region" grouping="wbRegion" title="Mean BMI Grouped By Region">}}

Looking at this, we can generally see that outside of the Sub-Saharan Africa,
South Asia, and East Asian & Pacific, regions, the countries of the world all
have an average BMI in the overweight or obese range.

Looking at the extreme ends of the BMI range, we can see that there are no countries
possessing an underweight average BMI.

> there are no countries possessing an underweight average BMI

At the same time, we can see that obesity has hit particularly hard to certain countries
in the East Asia & Pacific region. Looking more closely, the impact
of obesity has hit hardest in the Pacific Islands. Using the reasonable assumption
of a normal distribution, this means at least half of all men and women in the
countries of Nauru, Tonga, Samoa, and Palau are obese.

> at least half of all men and women in the countries of Nauru, Tonga, Samoa, and
Palau are obese

The only other country where this statement holds true is Kuwait, although there
are many other countries that are just shy of making the cut. For example, here in my
home country the U.S of A, male and female are only about 1 BMI point away.

## Results by income

Because there is a [relationship between obesity and socioeconomics]
(http://www.prb.org/Publications/Articles/2013/obesity-socioeconomic-status.aspx),
I also wanted to see if there was a visual pattern between a country's income and
its average BMI.

For reference the World Bank's income grouping:

Classification(2014) |  GNI / capita
-------------------- | --------------
Low income           |  <= $1045
Lower middle income  |  $1,046-$4,125
Upper middle income  |  $4,126-$12,735
Upper income         |  > $12,735

{{<highchartsTreeBMI src="/charts/bmi.json" metasrc="/charts/worldbank2014m.json" id="bmi-wb-income" grouping="income" title="Mean BMI Grouped By Income">}}

Through grouping countries by their income, we see a clear correlation between a
country's income and its average BMI.

> we see a clear correlation between a country's income and its average BMI

In the low income group, all countries have a normal average BMI except for Sudan
which is disqualified by only 0.2 points.

The lower middle income group has the greatest spread with about half being in
the normal range and half in the overweight or obese range. There needs to be
further research into this but I speculate that being above a certain income allows
countries to afford access to more "Westernized diets", which has been speculated
as a [potential contribution to weight gain]
(https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2990627/). This could be due to
being able to afford more industrial processing for food or perhaps just greater
importation. However this is all unfounded and requires further exploration.

In the upper middle and high income group, we once again see a nearly homogenous
pattern. Excluding what can be labelled as Asian countries and Angola, all of the
upper middle and high income countries possess an overweight or obese average BMI.

> Excluding what can be labelled as Asian countries and Angola, all of the
upper middle and high income countries possess an overweight or obese average BMI

A potentially interesting pattern I noticed were the countries where the average
BMI for male and female was split across normal and overweight. The average female BMI
was lower than the average male BMI in high income countries, but this trend was
reversed in upper middle income countries. Looking into this peculiarity of gender
differences actually led to me reading and writing quite a bit more than
anticipated, and will be in a second part as this post is already getting a bit long.

Before ending this post, here is the BMI plotted on a world map:

{{<highchartsMapBMI src="/charts/bmi.json" id="bmi-world-map" title="Mean BMI By Country 2014">}}

Unfortunately much of the Pacific Island countries do not show up on the map
perhaps due to their diminutive size but we can can still see the rest of
the world.

[Part 2 coming soon]

## Notes
- The data used is from 2014
- The direct link for the WHO dataset is broken. I worked around this by taking
the dataset used in their [Interactive Graph]
(http://gamapserver.who.int/gho/interactive_charts/ncd/risk_factors/bmi/atlas.html)
- I've sent an email to the WHO about the broken dataset but have yet to receive a response
