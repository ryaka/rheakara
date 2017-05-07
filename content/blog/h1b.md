+++
disqus = true
categories = [
]
date = "2017-05-05T13:47:49-07:00"
title = "Verifying H-1B Claims"
description = ""
hero = "/img/hello-world.jpg"
tags = [
]

+++

# Verifying H-1B Claims

The H-1B visa program has recently become a hot button topic. President Trump's
administration have made allegations that the program is being abused to replace
American workers with cheap labor. One claim the administration specifically
made is that "that about 80 percent of H1B workers are paid less than the median
wage in their fields".

> The result of that is that workers are often brought in well below market rates
> to replace American workers [Source](https://www.whitehouse.gov/the-press-office/2017/04/17/background-briefing-buy-american-hire-american-executive-order)

Nasscom, an Indian IT lobby, responded to accusations with saying that the workers
exported are highly skilled and that it is to meet a shortage in skills in the
United States.

## Methods

The data used for this comes from the US Department of Labor's disclosure on
the LCA program [here](https://www.foreignlaborcert.doleta.gov/performancedata.cfm).

The LCA is a document employers are required to fill out and get approved before
they can file for an H1-B visa. The purpose is to protect workers from being
taken advantage of and to protect American wages.

Because the USDOL does not publish the H-1B data directly, the LCA's are used as
a proxy to determine applications for the H-1B visas. The assumption rests on
employers filing an LCA will then proceed to file for an H-1B visa.

In addition only applications published in February and March are used because
I thought they'd be the most likely to proceed for an H-1B application which
opens in early April.

Initially I planned to use the data graciously published by a user off Kaggle
[here](https://www.kaggle.com/nsharan/h-1b-visa). Unfortunately some of the information
I wanted were removed in their sanitizing process so I proceeded to cleanse the
data myself. The process for that is published in this [post](google.com).

## Trends in H-1B applications

- **Applications increased 5 fold from 2010 - 2017** - Between 2010 and 2017,
the number of applications grew from an estimated 60,000 applications to
300,000. The bulk of this growth started in 2012 and continued up to 2016.

- **There was little to no growth from 2016-2017** - The number of applications
went from around 295,000 to 300,000, which is within the margin of error

{{<figure src="/img/num_position.png">}}

- **Computer / software related professions are hot** - The top
8 applied for positions as defined by the US government's SOC system, computer
and software positions make up at least 175,000 applications for 2017. This
makes up at least 60% of all applications.

{{<figure src="/img/perc_position.png">}}

- **There was a general decrease in the computer and mathematical sector** - Using
the general industry classification, the net number of H1B applications from this
group dropped about 10,000 from the previous year. As a whole the number of applications
dropped from around 71% of all applications to 67%.

{{<figure src="/img/perc_industry.png">}}

## Trends in top applicants

- **The 6 of the top 10 appliers for H-1B are based out of India** - Trump

| COMPANY                           | # Applications  | Adjusted Median Wage   |
|-----------------------------------|-----------------|------------------------|
| INFOSYS LIMITED                   | 147,579         | $76,859                |
| TATA CONSULTANCY SERVICES LIMITED | 71,915          | $69,457                |
| WIPRO LIMITED                     | 49,118          | $72,066                |
| DELOITTE CONSULTING LLP           | 42,793          | $91,315                |
| ACCENTURE LLP                     | 37,447          | $77,209                |
| IBM INDIA PRIVATE LIMITED         | 35,317          | $76,396                |
| MICROSOFT CORPORATION             | 29,884          | $118,968               |
| HCL AMERICA, INC.                 | 25,626          | $72,574                |
| TECH MAHINDRA (AMERICAS),INC.     | 23,603          | $74,007                |
| CAPGEMINI AMERICA INC             | 22,498          | $78,923                |

## Trends in wages

- Z
