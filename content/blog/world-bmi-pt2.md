+++
categories = []
date = "2016-10-04T14:55:19-07:00"
hero = "/img/pretty.jpg"
tags = []
title = "BMI Around the World Pt.2"
description = "A look at gender differences or: One way to discover cultural beauty standards"
draft = true
disqus = true
+++

[Part 1](/blog/world-bmi-pt1)

In my previous post I took a look at the average BMI around the world and one thing
that stood out to me was the extreme difference in male and female BMI in certain
countries. This in turn made me want to see how much difference there could be in
different countries around the world and if there was any skew in one direction or
the other. This is what this post will explore. I decided to make this into its
own post because the previous one was already getting a bit long and in order to
have a visual measurement, I had to change the way things were colored and scaled
and I didn't want any potential confusion with sudden change.

## The West is blue and the rest of the world is mostly red

For the scales used below, red indicates women have a higher BMI than men while
blue indicates that men have a higher BMI than women. The darker the color, the
more pronounced this difference. Roughly speaking, the more red the color, the heavier
the women / lighter the men, and the more blue the color, the lighter the women /
heavier the men.

{{<highchartsMapBMI2 src="/charts/bmi.json" id="bmi-world-map" title="Mean BMI Difference By Country 2014">}}

{{<highchartsTreeBMI2 src="/charts/bmi.json" metasrc="/charts/worldbank2014m.json" id="bmi-wb-region" grouping="wbRegion" title="Mean BMI Difference By World Bank Region">}}

Immediately there is a clear visual divide between European countries and the rest of the
world. Coming from the United States, my initial explanation for the matter was
due to beauty standards.

>there is a clear visual divide between The West and the rest of the world

I was no stranger to the beauty standard that thin is beautiful. And amongst one
Huffington Post writer, it was unsurprising to also find that trait be considered
beautiful in Europe.

>[I was unsurprised to find that in these three different cities the tall, thin, blonde archetype was the dominant ideal](http://www.huffingtonpost.com/antonia-opiah/how-women-in-europe-define-beauty_b_8206644.html)

In regards to this, we can see that Swiss women not only fight the odds greatest,
within their own country, but also throughout the rest of Europe for being the
thinnest. Nevertheless, European countries have thinner women and it may be because
of beauty standards.

Looking at the rest of the world...

## The red world

The thing more prominent that the divide was how enunciated the difference was in
some countries. If beauty standards was to be the reason for the gender difference
in Europe, it'd be best to remain consistent and see if it was also beauty standards
that explained women being heavier than men in the rest of the world.

## A look at the red: Sub-Saharan Africa, Western Africa

Looking up information about beauty in countries located in this area gave results
on beauty standards in Western Africa. I found an article by the IB Times which
spoke about how in Ghana and West Africa in general, women desire to be larger.

>[Indeed, like the rest of West Africa, Ghanaian women aspire to voluptuousness, even purchasing “appetite stimulants” in order to develop large busts, big behinds and thick legs](http://www.ibtimes.com/fat-land-western-standards-beauty-clash-west-african-notions-843573)

I also got to learn the extreme lengths which this was carried out in one of the
West African country of Mauritania. As it was in the IB Times article, I saw
information that reinforced the beauty standard that larger was beautiful.

>[Mauritanian tradition holds that among women, rolling layers of fat are the height of sexiness]
(http://www.marieclaire.com/politics/news/a3513/forcefeeding-in-mauritania/)

Unfortunately, I discovered that this standard is taken to an extreme in some cases
through the form of "fat camps" where girls are forced into the practice of
gavage, eating up to 16,000 calories a day. My brother who is a body builder
often complains and struggles to eat the 4,000 calories a day necessary so it
astounded me how this was possible. An interview with one of the "feeders"
quickly cleared it up.

>[How do small girls eat these gargantuan amounts of food? "I'm very strict,"
boasts Elhacen. "I beat the girls, or torture them by squeezing a stick between
their toes. I isolate them and tell them that thin women are inferior.]
(http://www.marieclaire.com/politics/news/a3513/forcefeeding-in-mauritania/)

## A look at the red: Middle East & North Africa

I found a study speculating the increase in weight in this particular regin. In
particular

>[The influence of men in determining women's attitudes towards body size is
another important issue in some countries in the region. In Qatar, for example,
about 43% of Arab women studied believed that men preferred plump women.
Similar findings were reported in Morocco, as there is a cultural preference of
body fatness among women of the Sahraoui ethnic group.]
(https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3175401/)

Heavy speculation. Also resorted to drugs

>[About 70% of South Morocco women had made a previous attempt to gain weight.
Appetite stimulant, overeating, and corticosteroids were the main methods used
to fatting. In addition, some women used traditional suppositories called Ligue,
composed of dates mixed with seeds and medicinal part, specifically for increasing
their peripheral fat [122]. It is believed that the preference for plumpness women
in some regions in the EMR countries is due to sexual attraction, rather than
any other factors. However, such conclusion needs to be studied.]
(https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3175401/)

## A look at the red: Carribean

Unable to find Dominica and Grenada specifically but was able to find Jamaica. Given
relative GDP and physical proximity very possible that the two former share similar
values with Jamaica. Also preferred heavier and also had resorted to taking drugs.

>["Women take the chicken pills to get broader hips and bigger bottoms," says
Carol's son Jason. "In our Jamaican culture, we love a girl that has a lot of shape."]
(http://www.npr.org/templates/story/story.php?storyId=124700865)

## A look at the red: Pacific

Unable to find comprehensive but saw some statements from PM remarking his
attitude and perceived attitudes of others in the region.

>["In Samoa, when a girl with big legs, big thighs and big everything walks by,
the old women will say, oh, what a beautiful girl...Us in the Samoa and the
Pacific Islands, it's certainly the big healthy voluptuous girl”]
(http://www.stuff.co.nz/life-style/beauty/9245664/Samoan-PM-says-big-is-beautiful)

## America is the most equal

Can't talk about inequality without equality. This was calculated by taking
the absolute value of the gender difference and subtracting it from a maximum.
The lower the difference, the greater the value. The color scale uses a white to
black gradient where the darker it is, the less the difference / greater the BMI
equality.

Looking at this America is the country with the greatest equality with there being
no difference between the mean BMI between men and women. However this is maybe not
too great as they both have a value of 28.8 which means the average American is
only about a point or so away from being considered obese.

>America is the country with the greatest equality with there being
no difference between the mean BMI between men and women. However this is maybe not
too great as they both have a value of 28.8 which means the average American is
only about a point or so away from being considered obese.

{{<highchartsTreeBMI3 src="/charts/bmi.json" metasrc="/charts/worldbank2014m.json" id="bmi-wb-income-eq" grouping="income" title="Mean BMI Equality By World Bank Income Group">}}

However looking at this it looks as if there is inequality towards one gender or the
other regardless of income. I took a look at the percentiles within these different
groups and they all did not seem too skewed one way or the other. Except that that
low income countries may be more particularly equal in BMI at higher end.

```
Classification         25%   50%   75%
======================================
Low income             3.3   3.8   4.6
Lower middle income    3.2   3.8   4.3
Upper middle income    3.4   3.8   4.2
High income            3.3   3.7   4.3
```

## Conclusions and caveats

Although beauty standards may explain factors in some of this, it is not Absolute
not universal. In the case of BMI difference in European country, it is possible
that many of the countries are within a defensible margin since it's arguable
the BMI should be [adjusted up by 2 points for men](http://halls.md/bmi-difference-men-women/).

I don't deny that there is a beauty standard but as far as just looking at the
numbers there needs to be some room for skepticism at using these numbers as a form
of implication.

In addition, it may not be all beauty standards and some of it may just be due to
["eating more like the Western World"](http://www.iol.co.za/lifestyle/big-is-beautiful-say-fat-south-africans-1412306)
As seen in the previous post, there seems to be a transitional area economically
where once a country hits lower middle income, they have possibility to become
overweight or obese, possibly due to this.

Nevertheless although there is no universality and beauty standards and body weight
and health is a complex matter, looking purely at these numbers allowed me to
discover beauty standards, culture, and practices I did not know of before. This
was both bad and good as although I got to learn about a greater range of what may
be deemed beautiful, I also learned about not so pleasant practices such as the
fat camps the girls in Mauritania were forced to go to to be force fed or women
in a variety of other countries taking medication to induce gain.

>looking purely at these numbers allowed me to
discover beauty standards, culture, and practices I did not know of before. This
was both bad and good as although I got to learn about a greater range of what may
be deemed beautiful, I also learned about not so pleasant practices such as the
fat camps the girls in Mauritania were forced to go to to be force fed or women
in a variety of other countries taking medication to induce gain.

<!-- {{<highchartsTreeBMI2 src="/charts/bmi.json" metasrc="/charts/worldbank2014m.json" id="bmi-wb-income" grouping="income" title="Mean BMI Difference By World Bank Income Group">}} -->
