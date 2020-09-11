---
title: "Documentation"
teaching: 0
exercises: 0
questions:
- "Key question (FIXME)"
objectives:
- "First learning objective. (FIXME)"
keypoints:
- "First key point. Brief Answer to questions. (FIXME)"
---


Documentation is essential for understanding and (re) using data:

Data specific information: what does this number represent, what units is it in, is it a time average, what is the relation between 2 datapoints (subsequent in time, distinct in space, same or different variable), etc.

Project information: how was the data obtained (where there steps)? By whom? Are there different versions of the data? Quality assurance?

On data specific info you often find difficult terms like ‘semantics’, ‘vocabularies’, ‘ontologies’, ‘linked data’. In climate (related) science, these are often so ‘logical’ that you won’t even notice they’re there. However, look at this example of a patient’s data model, and the netcdf model. Do you see it now? More info on this in sections file format and metadata.

Project info is typically written in the data description fields, but may also include pointers to external documents, such as the data management plans.

Point forward to next episodes (e.g. formats and metadata help to document data).

Data management plan describes the planning/methods of data collection activities, data processing, analysis and (long-term) preservation.

You can also log other important decisions that impact your data (sort of labjournal?!).

Documentation can take many forms: data management plan, papers published, (jupyter) notebooks, provencance information, etc. It is a good idea to bundle these with the data when you publish the data, so that people that find your data will not have to search for it elsewhere

{% include links.md %}

