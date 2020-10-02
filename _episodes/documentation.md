---
title: "Documentation"
teaching: 0
exercises: 0
questions:
- "What is documentation?"
- "What should I document when I process data?"
- "In which ways can I document my research data?"
objectives:
- "Ensure that others can re-use your data by having a clear data management plan."
- "Differentiate between project and data-level documentation."
- "Evaluate existing data documentation with a critical view towards reusability"
keypoints:
- "Documentation is meant to be read and understood by humans."
- "Documentation adds richer contextual information than metadata."
---


What is documentation?
----------------------

Documentation is about **Accessibility** and **Reusability**

Documentation is essential for understanding and (re) using data:

Data specific information: what does this number represent, what units is it in, is it a time average, what is the relation between 2 datapoints (subsequent in time, distinct in space, same or different variable), etc.

Point forward to next episodes (e.g. formats and metadata help to document data).

Documentation can take many forms: data management plan, papers published, (jupyter) notebooks, provencance information, etc. It is a good idea to bundle these with the data when you publish the data, so that people that find your data will not have to search for it elsewhere


What is the difference between documentation and metadata?
----------------------------------------------------------


Data-level documentation
------------------------

Data management plan describes the planning/methods of data collection activities, data processing, analysis and (long-term) preservation.

You can also log other important decisions that impact your data (sort of labjournal?!).


Project-level documentation
---------------------------

Project information: how was the data obtained (where there steps)? By whom? Are there different versions of the data? Quality assurance?

On data specific info you often find difficult terms like ‘semantics’, ‘vocabularies’, ‘ontologies’, ‘linked data’. In climate (related) science, these are often so ‘logical’ that you won’t even notice they’re there. However, look at this example of a patient’s data model, and the netcdf model. Do you see it now? More info on this in sections file format and metadata.

Project info is typically written in the data description fields, but may also include pointers to external documents, such as the data management plans.




{% include links.md %}

