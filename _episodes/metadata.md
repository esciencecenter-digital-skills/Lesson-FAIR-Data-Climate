---
title: "Metadata"
teaching: 0
exercises: 0
questions:
- "Key question (FIXME)"
objectives:
- "First learning objective. (FIXME)"
keypoints:
- "First key point. Brief Answer to questions. (FIXME)"
---


“Metadata are data about data. Research data need metadata to become findable, accessible, interoperable and reusable - by humans and machines. “

Conventions for metadata (CF, CMIP, )

Geospatial data

Example convention/standards hierarchy: NetCDF > CF conventions > CMIP conventions

Software can be useful to force you to adhere, e.g. many packages (like xarray in python) handle NetCDF files, Iris makes your data adheres to CF conventions, CMOR makes your data adhere to CMIP conventions. Units packages (cf_units?).

What about CDO/nco, gdal?

ESMValTool also has built in convention checkers: this ensures your data adheres to the standards.

Other forms of data (spectral, point data, image)

{% include links.md %}
