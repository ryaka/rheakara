+++
categories = []
date = "2016-10-03T14:44:46-07:00"
hero = "/img/food.jpg"
tags = []
title = "BMI Around the World Pt.1"
description = "Taking a look through different lenses"
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

With all of this in mind I wanted to get a visual representation of this information.

## Results by region

As a quick reference the BMI classifications are as follows:

```
Classification   Range       Color
===============================================
Underweight      < 18.5      dark purple-purple
Normal weight    18.5–24.9   blue-green
Overweight       25–29.9     orange-red
Obesity          > 30        red-black
```

The graphs use a colored scale to indicate where a country falls in these
categorizations. They are generated using a combination of country measurements
reported by the WHO, and regional and income classifications as published by
the World Bank.

As a note the WHO provides their own regional classifications for countries
but I quickly found it confusing with some of the classifications such as
*South-East Asia* having the very unexpected memberships of: *Maldives, Bhutan,
Sri Lanka, Nepal, India, Bangladesh, and North Korea*.

Using the World Bank's regional grouping:

{{<highchartsTreeBMI src="/charts/bmi.json" metasrc="/charts/worldbank2014m.json" id="bmi-wb-region" grouping="wbRegion" title="Mean BMI By World Bank Region">}}

Looking at this, we can generally see that outside of the Sub-Saharan Africa,
South Asia, and East Asian & Pacific, classifications, the countries of the world all
have an average BMI putting them in the overweight or obese range.

Looking at the extreme ends of the BMI range, we can see that there are no countries
possessing an average BMI in the underweight range.

> there are no countries possessing an average BMI in the underweight range

On the other end, we can see that obesity has hit particularly hard to certain countries
in the East Asia & Pacific classification. Looking more closely, the impact
of obesity has hit hardest in the Pacific Islands. Taking the reasonable assumption
of a normal distribution, this means at least half of all men and women in the
countries of Nauru, Tonga, Samoa, and Palau are obese.

> at least half of all men and women in the countries of Nauru, Tonga, Samoa,
and Palau as obese

The only other country that is hit as equally hard with this is Kuwait, although there
is no shortage of countries just barely straddling that line. For example, here in my
home country the U.S of A, men and women are only about 1 BMI point away from being
in the same group.

## Results by income

Given that there is a [relationship between obesity and socioeconomics]
(http://www.prb.org/Publications/Articles/2013/obesity-socioeconomic-status.aspx),
there is a strong pull to see if there is a visual pattern.

For reference the World Bank's income grouping:

```
Classification(2014)   GNI / capita
=====================================
Low income             <= $1045
Lower middle income    $1,046-$4,125
Upper middle income    $4,126-$12,735
Upper income           > $12,735
```

{{<highchartsTreeBMI src="/charts/bmi.json" metasrc="/charts/worldbank2014m.json" id="bmi-wb-income" grouping="income" title="Mean BMI By World Bank Income Group">}}

Grouping the countries by their income classification there seems to be a clear
relationship between a country's GNI per capita and its average BMI.

>Grouping the countries by their income classification there seems to be a clear
relationship between a country's GNI per capita and its average BMI

In the low income end, all countries are within the normal range except for Sudan
which is just barely above the line by 0.2 points.

The lower middle income group has the greatest spread with about half being in
the normal range and half in the overweight or obese range. There needs to be
further research into this but I speculate that being above a certain income allows
countries to afford access to more "Westernized diets" which has been speculated
as a [potential contribution to weight gain]
(https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2990627/). This could be due to
affording more industrial processes for food or perhaps just greater importation.
However this is all unfounded and leaves room for further exploration.

Exiting these two classifications we once again see a homogenous pattern. Excluding
what can be labelled Asian countries and Angola, all of the upper middle
and high income countries are consistently overweight or obese. This may leave room
for study in the countries of South Korea, China, Japan, Singapore, Thailand,
China, and Angola, and if there is any trend for them to join the rest.

>Excluding what can be labelled Asian countries and Angola, all of the upper middle
and high income countries are consistently overweight or obese

A potentially interesting pattern I noticed were in the countries where the average
BMI were split between between normal and overweight. Within the high income
countries where this occurred, the female's was lower than the male's, but this
trend was reversed in upper middle income countries. This actually gave me subject
matter to look into on a follow-up post in a part 2.

Before finishing this post, here is the BMI plotted on a world map:

{{<highchartsMapBMI src="/charts/bmi.json" id="bmi-world-map" title="Mean BMI By Country 2014">}}

Unfortunately much of the Pacific Island countries do not show up on the map
perhaps due to their diminutive size but we can can still see the rest of
the world.

[Part 2 coming soon]

## Notes
- I've sent an email to the WHO about the broken dataset but have yet to receive a response
