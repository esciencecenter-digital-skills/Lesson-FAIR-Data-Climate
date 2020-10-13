---
title: "Data licenses"
teaching: 20
exercises: 10
questions:
- "What is a data license?"
- "Which data license should I use for climate data?"
- "What are the consequences of (not) using a data license?"
- "Who decides which license I can use?"
objectives:
- "Find existing license policies that may apply to your data"
- "Choose a suitable license given these constraints"
- "Apply a license to your data"
keypoints:
- "A permissive license ensures the re-usability of your data."
- "Many big inter-comparison projects already have suitable licenses."
- "For derived work, existing licenses may restrict your choice of license."
- "Ownership of data (FIXME)"
---

General info on licenses
------------------------

Let's get started with a small exercise.

> ## Choosing a license
> Go to <https://chooser-beta.creativecommons.org/> and follow the steps.
>
>- What license did you arrive at?
>- Does the license fit with the FAIR principles?
>- Discuss.
{: .challenge}

One of the key parts of FAIR data is that they are **reusable** not only practically, but also legally. By attaching a license to your work, you specify who can reuse your data, for which purposes, and what should be done with derived work. Creative Commons (CC) are the most used license in research. They are widely recognized, easy to apply, and juridically sound. The CC license is built on four cornerstones:

- Attribution (BY): Credit must be given to you, the creator.
- Share-Alike (SA): Adaptations must be shared under the same terms.
- Non-Commercial (NC): Only noncommercial use of your work is permitted.
- Non-Derivative (ND): No derivatives or adaptations of your work are permitted.

The six CC licenses are combinations of these cornerstones.

> ## Note
> Without a license you keep the copyright to yourself. This prohibits anyone from using the data for their own work.
{: .callout}

These are some points to consider when choosing a license:

- A license cannot be revoked once the data has been shared.
- As the original author, you can change the license for future publications.
- Sensivite data / embargo
- The less restrictions you add to your data, the more it can be re-used

Further reading:
- <https://www.dcc.ac.uk/guidance/how-guides/license-research-data>
- <https://www.openaire.eu/research-data-how-to-license/>

> ## Discussion
>- When was the last time you published some data?
>- What license did you distribute it under?
>- Where did you share the data?
{: .discussion}

licenses in Geoscience
----------------------

In general, data sources in geoscience such as CMIP5 and CMIP6 are available under FAIR licenses. That is, you can freely use the data, but there are still some requirements. For example, if you base your research on CMIP6 data, you must give proper credit to the project if you deposit your research data somewhere. This is specified in the Terms of Use.

You can find the Terms of Use for some widely used projects here:

- CMIP6: <https://pcmdi.llnl.gov/CMIP6/TermsOfUse/TermsOfUse6-1.html>
- CMIP5: <https://pcmdi.llnl.gov/mips/cmip5/terms-of-use.html>
- CORDEX: <http://is-enes-data.github.io/cordex_terms_of_use.pdf>

>## Discussion
>- How do the terms of use for CMIP6 data differ from the Creative Commons licenses?
>- Can you reshare the data?
>- Should you attribute the authors of the data? If so, how?
>- Can derived data be used commercially?
>- Can you find additional terms of licenses that are applicable to your situation?
>- **FIXME**: check what the answer should be
{: .discussion}

Further reading:
- <https://gmd.copernicus.org/articles/11/3659/2018/> (Section 4)

Data ownership
--------------

One of the major challenges with data licenses is data ownership. Who actually owns the data? Can other parties use the data and what control do you have over the data as the owner? These points are addressed by the license file.

For any academic institute, there are three possible owners of the data:
- You
- Institute you work for
- Funding agency

Data ownership is defined in the data management plan. You may be restricted by your institutions’ policies on licenses.

> ## Excercise
>Take a few minutes to find out whether your institute has a license policy.
>
>- What does it say?
>- Who owns *your* data?
>- What do you do if your institution does not have a policy?
{: .discussion}

> ## Excercise
> Imagine, some researchers have SOME CRAZY EXAMPLE
>
> They have deposited the data on their institute's website under the data under CC-BY 4.0.
>
>- Do you see any problems with the license they chose?
>- Which data license should you put on it when you distribute the data?
>- Which license can you not put on it when you distribute the data?
{: .discussion}

What does the EU require?
-------------------------

The European Commission has fully embraced FAIR principles. Horizon2020 already mandates open access to all scientific publications, and is now running a pilot from 2017 for research data to be open by default with possibilities to opt-out.

How the data will be licensed is part of the data management plan. Specifically:

- How will the data be licensed to permit the widest re-use possible?
- When will the data be made available for re-use (i.e. are the data under embargo)?
- Are the data usable by third parties (i.e. are there restrictions)?

> ## Excercise
>Which license does the European Commission recommend for data acquired under the Horizon 2020 Programme?
>
>> ## Solution
>>The European Commission encourages researchers to provide access to their data in the broadest sense.
>>They encourage authors to retain their copyright, but grant adequate licenses to publishers.
>>They recommend the Creative Common licenses as a useful legal tool for providing open access.
>{: .solution}
{: .discussion}

Further reading:
- <https://ec.europa.eu/research/participants/docs/h2020-funding-guide/cross-cutting-issues/open-access-data-management/open-access_en.htm>
- <https://ec.europa.eu/research/participants/data/ref/h2020/other/hi/oa-pilot/h2020-infograph-open-research-data_en.pdf>
- In case you are really interested, have a look at [p251-253 of the Horizon2020 Programme](https://ec.europa.eu/research/participants/data/ref/h2020/grants_manual/amga/h2020-amga_en.pdf)

How are licenses applied to research data?
------------------------------------------

In principle, a license is valid when it is mentioned or referred to in the same place where you upload your data. Some repositories like Zenodo allow you to select a license, and they make sure it is clear under which license the data are available.

You can apply a license by one of these ways:

- Choosing a license when you upload your data to a repository
- Referring to the license on the webpage where the data are hosted
- Attaching the license to the metadata
- Adding a readme file / license file to your data

The [license chooser](https://chooser-beta.creativecommons.org/) can help you generate a plain text or html snippet to add to your readme or website.

> ## Note
> Specific to climate-related research, CMIP6 explicitly requires you to add the license to the metadata
{: .callout}

{% include links.md %}
