---
title: "Access to the data"
teaching: 10
exercises: 15
questions:
- "What is meant by 'accessibility'?"
- "What are relevant data repositories in climate science?"
- "How to choose a data repository?"
objectives:
- "Identify suitable repositories to make your research data acessible."
- "Plan access to the data in a data management plan."
keypoints:
- "Accessible does not mean open without constraint."
- "Metadata can still be accessible, even if the data itself is not (anymore)."
- "EU-funded projects are expected to make generated data accessible to the public."
---


## What is access to data?

Accessibility addresses the *A* in the FAIR principles. Once the user finds the required data, she/he needs to know how can they be accessed, possibly including authentication and authorisation. Accessible data objects can be obtained by humans and machines upon appropriate authorisation and through a well-defined and universally implementable protocol. In other words, anyone with a computer and an internet connection should be able to access at least the metadata.

> ## This is what [go-FAIR.org](https://go-fair.org/principles) has to say about Accessible
> - A1. (Meta)data are retrievable by their identifier using a standardised communications protocol
> - A1.1 The protocol is open, free, and universally implementable
> - A1.2 The protocol allows for an authentication and authorisation procedure, where necessary
> - A2. Metadata are accessible, even when the data are no longer available
{: .checklist}

> ## Accessible does not mean open without constraint
> Accessibility means that the human or machine is provided - through metadata - with the precise conditions by which the data are accessible and that the mechanisms and technical protocols for data access are implemented such that the data and/or metadata can be accessed and used at scale, by machines, across the web.
{: .callout}


Repositories: domain-specific versus generic
btw: repos also relevant for other aspects of FAIR (e.g. they help to find data).


Exercises:

Stages of accessibility.
You are asked to make data accessible. Hence,

- you make a note in your paper that data can be requested by sending you an email
- you provide the data as supplementary information to your paper
- you upload the data to dropbox and put a shareable link in your paper
- you upload the data to a university drive and request a DOI from the library
- you upload the data to a generic repository such as zenodo
- you upload the data to a domain-specific repository such as hydroshare

Describe whether or not this is adhering to the FAIR principles.


Let's examine a couple of different data repositories (maybe datasets in different repos?)
For each of the repositories listed ..., answer the following questions:

- Is this repository publicly accessible?
- Is it free?
- Is it proprietary?
- Does it allow for authenthication?
- Is there any quality control for this repository?
- Are metadata accessible, even if the data is not?
- How long will the data be maintained?
- Is there any backup system in place?
- Is it easy to find data that is stored in this repository?
- Is it easy to download data from this repository?
- Is it easy to upload data to this repository?

Discussion: When it comes to making data accessible, there are some easy steps
that can by applied by any researcher to their own data. Some steps, however,
have to be developed accross a scientific domain. Particularly, the
establishment of domain-specific data repositories. What is the status in your
specific (sub) domain? Is/are there suitable repositories, and are they easy to
use? Or is there still room for improvement?


How long should data be acessible?


## How to access data

- ESGF, first choice for any climate scientist?

- CDS, ??

- Climate4Impact for less technical audience

- Zenodo, (or other repositories)
    Small peace about zenodo and how to use it

- Website of a dataset

    Although FAIRness in climate science is advancing and some clearly accessible repositories exist, it is still also common practice to only make a dataset accessible via the project website. Because projects do not last for ever, some of these websites are not maintained, resulting in inaccessible datasets.

- Machine access through well described protocols and metadata


> ## Exercise
> For the following three datasets, find out how you can access them:
> - ?
> - ?
> - ?
{: .challenge}

> ## Discussion
> Often accounts are needed to access CMIP data on ESGF.
> - Why do you think this is?
> - What are the advantages/disadvantages of this approach?
{: .challenge}

## I have created data, how do I make it accessible


{% include links.md %}
