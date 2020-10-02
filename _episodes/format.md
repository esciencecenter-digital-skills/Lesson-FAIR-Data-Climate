---
title: "File format"
teaching: 0
exercises: 0
questions:
- "What is a file format?"
- "What file formats should I use?"
-
objectives:
- "Name common formats used in climate-related domains."
- "Understand different types of data."
- "Choose correct file formats for your work."

keypoints:
- "Choose formats that are common to your field/community."
- "Decide on how long do you intend to preserve your data."
- "Use a common, multi-platform file format."
- "Make sure to check requirements of the repository where data is stored."
---

## File format

A [file format](https://en.wikipedia.org/wiki/File_format) is the structure of a file.
It determines how the data within the file is organized.
A File format is also called a file extension.
Files are usually named as `filename.format`.
For example, climate.jpeg is a file named climate with [jpeg](https://en.wikipedia.org/wiki/JPEG) format.
You might know that `jpeg` is a commonly used format for digital images.
Therefore, the file `climate` is an image.

## Common file format in climate-related domains

In climate-related domains e.g. weather and climate science, Earth observation science, hydrology,
data can be in many types and for different purposes.
In this section, we will learn about the common formats of data.

> ## Common file format in your community/research team
>
> You work with some data for a project in your community.
>
> 1. What is the format of the data?
> 2. Do you know why the data is in that format?
>
{: .discussion}

Here is a list of some common formats:

- [NetCDF](https://www.unidata.ucar.edu/software/netcdf/docs/netcdf_data_model.html)

  It was originally developed for the Earth science community, but it can be used for many kinds of data.
  NetCDF views the world of scientific data in the same way that a geo-scientist might:
  ![NetCDF]({{ page.root }}/fig/netcdf-classic-uml.png)

  There are various quantities such as temperature or elevation
  located at points at particular coordinates in space and time.

  The quantities (here temperature or elevation) are stored as netCDF variables.
  Variables are N-dimensional arrays of data, with a name.

  The coordinates information are stored as netCDF dimensions.
  Dimensions have a length and a name.

  A scientist also wants to store supporting information or metadata, such as the units, or
  some information about how the data were produced.
  The metadata is stored as netCDF attributes that are always single values or one-dimensional arrays.

> ## View a NetCDF file
>
> FIX ME
> > ## Solution
> >
> >
> {: .solution}
{: .challenge}

- [GRIB](https://www.wmo.int/pages/prog/www/DPS/FM92-GRIB2-11-2003.pdf)
GRIB stands for general regularly-distributed information in binary.
![GRIB]({{ page.root }}/fig/grib-form.png)

> ## View a GRIB file
>
> FIX ME
> > ## Solution
> >
> >
> {: .solution}
{: .challenge}

- [GeoTIFF]

> ## View a GeoTIFF file
>
> FIX ME
> > ## Solution
> >
> >
> {: .solution}
{: .challenge}

- [HDF5]

> ## View a HDF5 file
>
> FIX ME
> > ## Solution
> >
> >
> {: .solution}
{: .challenge}

> ## Other formats
>
> What about other formats like TIFF, GIS-applications,
> Vector data (e.g. shapefiles), netcdf-zarr-data-model etc?
{: .callout}

## Different formats for different purposes

what file formats to use for each purpose: data collection/ processing/analysis, reuse, and preservation

## Different formats for different types

what file formats to use for each type: geospatial, tabular, storyline, documentation and paper, textual, video/audio, image/figure

> ## non/proprietary format
>
> FIX ME
{: .callout}

{% include links.md %}
