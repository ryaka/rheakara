+++
disqus = true
categories = [
]
date = "2017-05-05T13:47:49-07:00"
title = "Checking H-1B Claims"
description = "Public draft..."
hero = "/img/h1b.jpg"
tags = [
]

+++

# Checking H-1B Claims

The H-1B visa program has recently become a hot button topic. President Trump's
administration have made allegations that the program has been abused to replace
American workers with cheap labor. One claim the administration specifically
made is that "that about 80 percent of H1B workers are paid less than the median
wage in their fields".

> The result of that is that workers are often brought in well below market rates
> to replace American workers [Source](https://www.whitehouse.gov/the-press-office/2017/04/17/background-briefing-buy-american-hire-american-executive-order)

Nasscom, an Indian IT lobby, responded to accusations by stating that the workers
exported are highly skilled and that it is to meet a shortage in skills in the
United States.

Given that the issue is a hot political topic with contradicting assertions on
both sides, I wanted to take a look at the available data and try to make some
conclusions for myself.

## Methods

The data used for this comes from the US Department of Labor's disclosure on
the LCA program [here](https://www.foreignlaborcert.doleta.gov/performancedata.cfm).

The LCA is a document employers are required to fill out and get approved before
they can file for an H-1B visa. The purpose is to protect workers from being
taken advantage of and to protect American wages.

Because the US DOL does not publish the H-1B data directly, the LCA's are used as
a proxy to determine applications for the H-1B visas. The method rests on the
assumption that employers filing an LCA will likely proceed to file for an H-1B visa.

In addition, only LCA applications submitted in February and March are used. This
is because H-1B applications have historically opened in early April. These two
months are close enough to it that I believe there is a high correlation of the
LCA applications submitted in this time period being submitted to H-1B. Some
back of the envelope calculations also seem to give decent numbers. At the very least
the general trends and compositions should be the same.

{{<figure
  src="/img/h1b_month_2016.png"
  caption="Submissions spike in February and March">}}

As a quick aside, I initially planned to use data graciously published by a user
off Kaggle [here](https://www.kaggle.com/nsharan/h-1b-visa). Unfortunately some of the
information I wanted were removed in their sanitizing process so I proceeded to
cleanse the data myself. The process for that is published in this [post](google.com).

## General Trends in H-1B applications

### Applications increased 5 fold from 2010 - 2017

{{<figure
  src="/img/num_position.png">}}

Between 2010 and 2017, the number of applications grew from an estimated 60,000
applications to 300,000. The bulk of this growth started in 2012 and continued
up to 2016.

### There was little to no growth from 2016-2017

The number of applications went from around 295,000 to 300,000, which is within
the margin of error.

### Computer / software related professions are hot

{{<figure
  src="/img/perc_position.png">}}

The top 8 applied for positions as defined by the US government's SOC system,
computer and software positions make up at least 175,000 applications for 2017.
This makes up at least 60% of all applications.

### There was a general decrease in the computer and mathematical sector

{{<figure
  src="/img/perc_industry.png">}}

The net number of H1B applications from this industry (using SOC classification)
group dropped about 10,000 from the previous year. As a whole the number of applications
dropped from around 71% of all applications to 67%.

## Trends in major applicants

IGATE TECHNOLOGIES INC., INTEL CORPORATION , IBM CORPORATION, AMAZON CORPORATE LLC,
DELOITTE & TOUCHE LLP are respectively omitted.

The White House recently made [accusations](https://www.whitehouse.gov/the-press-office/2017/04/17/background-briefing-buy-american-hire-american-executive-order) that some companies are abusing the H-1B system by flooding the
system with applications to get a disproportionate amount of visas. In addition
the companies "Tata, Infosys, Cognizant" were particular named in the accusations
as some of these abusers. Finally the workers being imported as alleged as
"actually less skilled and lower paid than the workers that they’re replacing".

Nasscom, an Indian IT lobby, [responded to accusations](http://www.business-standard.com/article/companies/tcs-infosys-got-only-8-8-of-total-h-1b-visas-nasscom-s-rebuttal-to-us-117042401271_1.html) by stating that the workers
exported are highly skilled and that the numbers merely fulfill a shortage
in skills in the United States.

### "Only six Indian IT firms were among the top 20 recipients of the H-1B visas in fiscal 2015"

| COMPANY (2015)                                          | APPLICATIONS   | MEDIAN WAGE (ADJUSTED) |
|---------------------------------------------------------|----------------|------------------------|
| 1. **INFOSYS LIMITED**                                  | 18204          | $73368                 |
| 2. **TATA CONSULTANCY SERVICES LIMITED**                | 8025           | $69865                 |
| 3. ACCENTURE LLP                                        | 5351           | $76846                 |
| 4. **IBM INDIA PRIVATE LIMITED**                        | 5169           | $76006                 |
| 5. **WIPRO LIMITED**                                    | 4471           | $69033                 |
| 6. DELOITTE CONSULTING LLP                              | 3130           | $82559                 |
| 7. **HCL AMERICA, INC.**                                | 2936           | $73497                 |
| 8. IGATE TECHNOLOGIES INC.                              | 2545           | $67905                 |
| 9. **TECH MAHINDRA (AMERICAS),INC.**                    | 2317           | $73669                 |
| 10. **LARSEN & TOUBRO INFOTECH LIMITED**                | 1714           | $72018                 |
| 11. ERNST & YOUNG U.S. LLP                              | 1649           | $79669                 |
| 12. MICROSOFT CORPORATION                               | 1531           | $122562                |
| 13. GOOGLE INC.                                         | 1467           | $123838                |
| 14. UST GLOBAL INC                                      | 1164           | $61919                 |
| 15. **COGNIZANT TECHNOLOGY SOLUTIONS U.S. CORPORATION** | 1035           | $68023                 |
| .....                                                   | ....           | ......                 |
| 20. AMAZON CORPORATE LLC                                | 662            | $113518                |

The data matches Nasscom's claim given above. Namely these companies would be
Infosys, Tata, IBM India, Wipro, Larsen & Toubro, and Cognizant.

However, **all of these companies are actually in the top 15** which increases the
relative weight. In addition if we also include companies that are merely
American based subsidiaries but India headquartered, this would include
HCL America and Tech Mahindra which means that **8 India-bodied IT firms are
among the top 15 applicants of H-1B visas for 2015**.

This trend is also upheld over the entire 2010 - 2017 period.

| COMPANY (2010-2017)                                     | APPLICATIONS   | MEDIAN WAGE (ADJUSTED) |
|---------------------------------------------------------|----------------|------------------------|
| 1. **INFOSYS LIMITED**                                  | 73770          | $75094                 |
| 2. **TATA CONSULTANCY SERVICES LIMITED**                | 29429          | $68730                 |
| 3. ACCENTURE LLP                                        | 19478          | $76287                 |
| 4. **WIPRO LIMITED**                                    | 18951          | $70385                 |
| 5. DELOITTE CONSULTING LLP                              | 17526          | $84743                 |
| 6. **TECH MAHINDRA (AMERICAS),INC.**                    | 16167          | $72890                 |
| 7. **IBM INDIA PRIVATE LIMITED**                        | 15220          | $76189                 |
| 8. **HCL AMERICA, INC.**                                | 11300          | $73649                 |
| 9. CAPGEMINI AMERICA INC                                | 10993          | $74400                 |
| 10. MICROSOFT CORPORATION                               | 9995           | $118232                |
| 11. ERNST & YOUNG U.S. LLP                              | 9948           | $80495                 |
| 12. GOOGLE INC.                                         | 8968           | $126000                |
| 13. **LARSEN & TOUBRO INFOTECH LIMITED**                | 7342           | $68469                 |
| 14. **COGNIZANT TECHNOLOGY SOLUTIONS U.S. CORPORATION** | 7337           | $69722                 |
| .....                                                   | ....           | ......                 |
| 20. UST GLOBAL INC                                      | 3852           | $63028                 |

### Top Indian IT firm applications peaked in 2015

The top 10 indian applicants reached a peak back in 2015 and as a net have
decreased tremendously in past 2 years. Infosys is perhaps the most dramatic,
dropping from a high of ~18,000 applications in 2015 to ~9,000 in 2017.

{{<figure src="/img/num_indian.png">}}

## Trends in wages

One of the accusations put forth by the White House has been that the workers
brought in by the supposed H-1B abusers are a form of cheap labor.

To check on these claims, the median wages for the top 5 positions brought over
by each of the top 6 Indian IT firms was calculated. In order to take geography
into account, the wages were were calculated for each city.

The heatmaps below show the wages and relative wages to the prevailing wage
for the top 5 positions in the top 5 worksite cities for each company. To reduce
variance, values are shown only if there are at least 10 such workers at each
worksite.

Exemplary heatmaps are chosen below to save space. A full gallery for all the
companies can be found [here](google.com).

### Top Indian IT Firm Workers Are Spread Out

{{<figure src="/img/num_wage_infosys.png">}}

Unlike some of the major tech names such as Google, Microsoft, etc. the majority
of Indian IT firms spread workers out all over the US rather than just a few
central metropolitan areas.

### Top Indian IT Firm Workers Are Paid Above the Prevailing Wage

{{<figure src="/img/perc_wage_infosys.png">}}

In regards to the prevailing wage (~market wage for a geography) provided by
H-1B employers, the workers brought in by the top Indian IT firms are paid
decently above the market.

## Not So Fast? Questions On The Wages.

Using the numbers provided by H-1B employers, the workers brought in to the
US seem to **not** be cheap labor being paid under market wages. However, during
this process, I ran across something strange. When we compare the wage maps between
the Indian IT firms and major household-name American firms such as Google,
Microsoft, etc. we see an extremely contrasted picture.

## Why Do Top Indian IT Firms Pay Significantly Below Top American Firms?

{{<figure src="/img/num_wage_google.png">}}

If we look at the wages for the American firms, the workers are consistently
paid significantly higher. It can be argued that, of course, these American firms
are the cream of the crop so they can afford to pay significantly higher. In addition
many of them are located in very expensive areas.

If we look at the percentage vs prevailing wage, we can see that the percentage
is not too different from many Indian IT firms.

{{<figure src="/img/perc_wage_google.png">}}

However......

## Why Do Top Indian IT Firms Apply Workers Under Such Different Positions?

{{<figure src="/img/perc_position_indian.png">}}

{{<figure src="/img/perc_position_big.png">}}

The values above were calculated by constraining positions to just 5 positions.
The number of applications for each company for each position was then calculated
and then weighted to get the relative percentage a type of position is filed
for to the rest.

For example, if company A had the following number of workers:
[12, 14, 29, 60, 16] then the values calculated would be
[12, 14, 29, 60, 16] / sum([12, 14, 29, 60, 16]).

We can see that Indian IT firms exceedingly do not file their workers under
[software developer](https://www.bls.gov/soc/2010/soc151132.htm), but instead
the workers are filed under [one](https://www.bls.gov/soc/2010/soc151199.htm) of
[several](https://www.bls.gov/soc/2010/soc151131.htm) [others](https://www.bls.gov/soc/2010/soc151121.htm).
This is **exceedingly contrary** to many of the top American firms.

## What Do These Title Differences Mean?

The titles used are from the [SOC] (https://www.bls.gov/soc/) codes filed with
every application.

As a person in tech, the titles of computer programmer and software developer
are mostly interchangeable with one another. To try and establish the difference,
I looked into the definitions but I was only further confused because many of the
tasks listed for a particular position seemed very like those in the others.

## Most Top Indian IT Firm Workers Are Underpaid If Compared to Workers Filed As Software Dev.

{{<figure src="/img/perc_wage_wipro_compare.png">}}

Rest of gallery [here](google.com).

If we compare these workers' wages to H-1B workers in the same geo, filed as a
[Software Developer, Applications] (https://www.bls.gov/soc/2010/soc151132.htm),
most of these tech firms would be paying a very large number of their workers. The
exception to this is IBM India and Tech Mahindra.

To be continued.... this is a draft

<!-- - **[Computer Occupations, All Other](https://www.bls.gov/soc/2010/soc151199.htm)** - All computer occupations not listed separately
- **[Computer Programmers](https://www.bls.gov/soc/2010/soc151131.htm)** - Create, modify, and test the code, forms, and script
that allow computer applications to run. Work from specifications drawn up by software
developers or other individuals. May assist software developers by analyzing user
needs and designing software solutions. May develop and write computer programs
to store, locate, and retrieve specific documents, data, and information.
- **[Computer Systems Analyst](https://www.bls.gov/soc/2010/soc151121.htm)** - Analyze science, engineering, business, and other data processing problems to implement and improve computer systems. Analyze user requirements, procedures, and problems to automate or improve existing systems and review computer system capabilities, workflow, and scheduling limitations. May analyze or recommend commercially available software.
- **[Software Developer, Applications](https://www.bls.gov/soc/2010/soc151132.htm)** - Develop, create, and modify general computer applications software or specialized utility programs. Analyze user needs and develop software solutions. Design software or customize software for client use with the aim of optimizing operational efficiency. May analyze and design databases within an application area, working individually or coordinating database development as part of a team. May supervise computer programmers.
- **[Software Developer, Systems Software](https://www.bls.gov/soc/2010/soc151133.htm)** - Research, design, develop, and test operating systems-level software, compilers, and network distribution software for medical, industrial, military, communications, aerospace, business, scientific, and general computing applications. Set operational specifications and formulate and analyze software requirements. May design embedded systems software. Apply principles and techniques of computer science, engineering, and mathematical analysis. -->
