---
title: "Documentation"
teaching: 5
exercises: 15
questions:
- "What is documentation?"
- "Where to document my data?"
- "What is the difference between documentation and metadata?"
objectives:
- "Evaluate existing data documentation with a critical view towards reusability"
- "Ensure that others can re-use your data by writing clear documentation."
keypoints:
- "Documentation provides rich contextual information mostly intended for human readers."
- "Documentation is essential for data reuse and reproducibility."
---

## What is documentation?

![https://xkcd.com/833/](https://imgs.xkcd.com/comics/convincing.png)
*Source: <https://xkcd.com/833/>*

Data documentation is all relevant information needed to properly interpret a
dataset. Documentation can be very specific about the data. For example, what
does this dataset represent, what units is it in, is it a time average, what is
the relation between 2 datapoints (subsequent in time, distinct in space, same
or different variable), etc. But, the documentation can also answer some
questions about the project: why were these data collected, by whom, and what
questions do they address? Was there any kind of quality assurance?

## Where to document my data?

Documentation can take many forms: a data management plan, papers published,
(jupyter) notebooks, lab journals, provenance information, etc. It is a good
idea to bundle these with the data when you publish the data, so that people
that find your data will not have to search for it elsewhere, and that access to documentation is guaranteed. Most data
repositories have a 'description' field, which is a suitable place to provide
any information that is not covered by the other metadata fields.

> ## Grouping related files with Zenodo communities
> Data documentation in your project may be scattered over many files of
> different types. To bundle this information, Zenodo allows you to upload
> a set of related files (hundreds if needed) as a single dataset.
>
> In addition, Zenodo provides 'communities'. You can upload all your datasets
> to Zenodo and add them to a community, thus keeping track of all relevant
> data for an entire project. You can also track versions. Each dataset
> gets its own DOI. So you could e.g. cite your data management plan
> in the description field of your dataset.
{: .callout}

## What is the difference between metadata and documentation?

Following <https://howtofair.dk>, we discuss data documentation and metadata
separately. However, the distinction between the two is not always clear. In
this episode, we will focus on the rich, descriptive kind of documentation
that is mostly relevant for human interpretation. In the next episodes, we will
focus on more formalized metadata that is also, or even mainly, intended for
machine readability.

## Exercises

> ## Checking data documentation
>
> Visit a data repository of your choosing (e.g. HydroShare, 4TU.ResearchData, Zenodo, ...).
> Select one or more datasets that you find interesting, and answer the
> following questions:
>
> - Is the title of the dataset entry in the repository clear and informative?
> - Is there a general description of the data?
> - Is there a reference to some external documentation of the data (e.g. a
>   journal publication)?
> - Would you be able to reproduce this data, based on the provided information?
> - Would you be able to use this dataset in your own (hypothetical) research
>   project?
> - Are contact details provided that you can use in case you have questions?
> - Is there any description of the context in which this dataset was created?
> - What could be improved about the documentation of this dataset?
{: .challenge}

> ## Writing your own data documentation
>
> For the real use case you selected in the previous episode, write a general
> description of the dataset(s) that will be produced. This description may
> include references to external documents. Also include the steps taken to
> obtain the final result ('data flow'). Make sure it will be adequate for
> others to understand how the data have been created. Also try to formulate a
> suitable title for the dataset(s).
>
> You may also write down some more technical aspects of the data, such as
> variable names, units, grids, creation date, software versions, etc.
>
> Limit your description to a single page (max).
{: .challenge}

## Further reading
- <https://guides.ucf.edu/metadata/dataDocumentation>

{% include links.md %}
