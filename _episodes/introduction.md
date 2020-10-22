---
title: "Introduction"
teaching: 5
exercises: 10
questions:
- "What are the FAIR principles?"
- "Why should I care to be FAIR?"

objectives:
- "Find relevant information on FAIR data requirements"
- "Express a vision on reproducible research"
- "Recognize possibilities for making a dataset more FAIR"

keypoints:
- "The FAIR principles state that data should be Findable, Accessible,
  Interoperable, and Reusable."
- "FAIR data enhance impact, reuse, and transparancy of research."
- "FAIRification is an ongoing effort accross many different fields."
- "FAIR principles are a set of guiding principles, not rules or standards." 
---

## What is FAIR?

FAIR is an acronym for Findable, Accessible, Interoperable, Reusable.
The FAIR principles for research data, originally published in a [2016 Nature
paper](https://doi.org/10.1038/sdata.2016.18), are intended as "a guideline for
those wishing to enhance the reusability of their data holdings." This guideline
has subsequently been endorsed by working groups, funding bodies and
institutions.

The FAIR principles have a strong focus on "machine-actionability".
This means that the data should be easily readable by computers (and not only by humans). This is particularly relevant for working with and discovering new data.

![FAIR principles illustration by Scriberia](../fig/FAIRPrinciples.jpg) *This
image was created by Scriberia for The Turing Way community and is used under a
CC-BY licence. Source: <https://doi.org/10.5281/zenodo.3695300>*

> ## FAIR is not open
>
> Some data cannot be shared openly, for example, because of privacy considerations.
> For such situations, the EU H2020 Program Guidelines on FAIR Data say that the data should be *"As open as possible, as closed as necessary."*
>
>
{: .callout}

## Why FAIR?

The original authors of the FAIR principles had a strong focus on enhancing
reusability of data. This ambition is embedded in a broader view on knowledge
creation and scientific exchange. If research data are easily discoverable and
re-usable, this lowers the barriers to repeat, verify, and build upon previous
work. The authors also state that this vision applies not just to data, but to
all aspects of the research process. This is visualized in the image below.

![Reproducibility illustration by Scriberia](../fig/ReproducibleJourney.jpg) *This
image was created by Scriberia for The Turing Way community and is used under a
CC-BY licence. Source: <https://doi.org/10.5281/zenodo.3695300>*

> ## What's in it for you?
>
> Many funders nowadays require from researchers data management plans which
> adhere to the FAIR principles. A great step forward, but if 
> we are going to spend the time and effort, we prefer to find some intrinsic 
> motivation.
>
> Have a look at the original [Nature paper](https://doi.org/10.1038/sdata.2016.18)
> on FAIR Data, the [GO-FAIR initiative](https://www.go-fair.org/fair-principles/),
> and the Danish tutorial [howtofair.dk](https://www.howtofair.dk/why-fair/).
> What are the main reasons for *you* to (not) embrace the FAIR principles?
{: .discussion}

## How FAIR are my data?
_AK: The title was a bit misleading; there isn't much about FAIRification process itself._

It is important to realize that the FAIR principles are not rules or standards.
They are a set of guiding principles, but their implementation may differ per
field or even per project. Since the principles have originally been established
only in 2016, a comprehensive set of specific requirements for FAIR data is
lacking for most fields.

In this tutorial, we will therefore interpret "FAIRness" as a continous scale
(less FAIR vs. more FAIR) rather than a binary classification (FAIR vs. not FAIR) (Mons et al., 2017).
Some steps can already be taken today, whereas other steps require the
development of standards across a scientific domain, or even changes to the funding model of projects.
We will aim to identify those quick wins and to facilitate the discussion on more involved developments.

> ## Select your case study for the tutorial
>
> In the tutorial we will be using real use cases to assess the FAIRness of a
> dataset and identify possibilities for improvement. Take a few minutes to find
> a suitable use cases. This may be one of your own projects or (recent) papers,
> or you may select another study you find interesting.
>
> Write down:
>
> - Any input dataset(s) that were used for this study
> - The methods, tools or models that were applied to these data
> - A short description of the output data that was generated
> - Additional information that you find relevant (e.g. the scientific domain,
>   project, journal, community)
>
> If you can't find a suitable project, you may use [the example paper by
> Glotter et al.](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4066535/) (which
> was randomly selected by the authors of this tutorial).
{: .challenge}

## Further reading

- Wilkinson et al. (2016) _The FAIR Guiding Principles for scientific data management and stewardship_. doi:[10.1038/sdata.2016.18](https://doi.org/10.1038/sdata.2016.18)
- Mons et al. (2017) _Cloudy, increasingly FAIR; revisiting the FAIR Data guiding principles for the European Open Science Cloud_. doi:[10.3233/ISU-170824](https://doi.org/10.3233/ISU-170824)
- [FORCE11](https://www.force11.org/fairprinciples)
- [GO FAIR initiative](https://www.go-fair.org/fair-principles/)
- [EU H2020 Guidelines on FAIR Data Management](https://ec.europa.eu/research/participants/data/ref/h2020/grants_manual/hi/oa_pilot/h2020-hi-oa-data-mgt_en.pdf)

{% include links.md %}
