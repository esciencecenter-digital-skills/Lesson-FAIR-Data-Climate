---
title: "File format"
teaching: 0
exercises: 0
questions:
- "What is a file format?"
- "What file formats should I use?"
objectives:
- "Name common formats used in climate-related domains."
- "Understand different types of data."
- "Choose correct file formats for your work."

keypoints:
- "Choose formats that are common to your field/community to ensure the interoperability and reusability of your data."
- "Make sure that the file formats you choose can hold the necessary data elements and information."
- "Decide on how long do you intend to preserve your data."
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

> ## Common file format for geospatial data in your community/research team
>
> You work with some data for a project in your community.
>
> 1. What is the format of the data?
> 2. Do you know why the data is in that format?
>
{: .discussion}

Here is a list of some common formats:

- [NetCDF](https://www.unidata.ucar.edu/software/netcdf/docs/netcdf_data_model.html):
  It was originally developed for the Earth science community, but it can be used for **many kinds of data**.
  NetCDF views the world of scientific data in the same way that a geo-scientist might:
  ![NetCDF]({{ page.root }}/fig/netcdf-classic-uml.png)

  - There are various quantities such as temperature or elevation
  located at points at particular coordinates in space and time.

  - The quantities (here temperature or elevation) are stored as netCDF variables.
  Variables are N-dimensional arrays of **data**, with a name.

  - The coordinates information are stored as netCDF dimensions.
  Dimensions have a length and a name.

  - A scientist also wants to store supporting information or **metadata**, such as the units, or
  some information about how the data were produced.
  The metadata is stored as netCDF attributes that are always single values or one-dimensional arrays.

> ## Why NetCDF format
>
> You work with some geospatial data for a project in your community.
> You choose the NetCDF format for the data.
> Your colleague asks:
>
> 1. Why did you choose the NetCDF format?
> 2. Does this format help to make the data FAIR?
>
>> ## Solution
>>
>> 1. You found that NetCDF format is the standard in your research community and
>> therefore interoperable and reusable for anyone.
>> Also, the NetCDF format can contain both data and metadata.
>>
>> 2. Therefore, yes, the NetCDF format helps to make the data FAIR.
> {: .solution}
{: .challenge}

- [GRIB](https://www.wmo.int/pages/prog/www/DPS/FM92-GRIB2-11-2003.pdf):
  GRIB stands for general regularly-distributed information in binary.
  It is **commonly used** by the [World Meteorological Organization](https://public.wmo.int/en)(WMO) for weather model data.

  - GRIB coded data consist of a continuous bit-stream made of a sequence of
  [octets](https://en.wikipedia.org/wiki/Octet_(computing)).
  Thus, the representation of the data is **independent of** any particular machine representation.

  - GRIB messages contain the **data** and **metadata**.

> ## Why GRIB format
>
> You work with some geospatial data for a project in your community.
> You choose the GRIB format for the data.
> Your colleague asks:
>
> 1. Why did you choose the GRIB format?
> 2. Does this format help to make the data FAIR?
>
>> ## Solution
>>
>> 1. You found that GRIB format is the standard in your research community and
>> therefore interoperable and reusable for anyone.
>> GRIB format is independent of any particular machine representation.
>> Also, the GRIB format can contain both data and metadata.
>>
>> 2. Therefore, yes, the GRIB format helps to make the data FAIR.
> {: .solution}
{: .challenge}

- [GeoTIFF](https://www.geospatialworld.net/article/geotiff-a-standard-image-file-format-for-gis-applications/):
  GeoTIFF is a standard image file format to describe and store raster image data with geographic information.
  So it can be used by  Geographic Information System (GIS) applications.

  - GeoTIFF format is suitable for a **wide range of applications worldwide**.
  For example, satellite imaging systems, scanned aerial photography, scanned maps,
  digital elevation models, or as a result of geographic analyses.

  - It is **independent** of a computer’s architecture, operating system, and graphics hardware.

  - GeoTIFF format has a three-level hierarchy: file header, image file directories, and **data**.

  - GeoTIFF format stores a **broad range of georeferencing information**, catering to geographic
  as well as projected coordinate systems.

> ## Why GeoTIFF format
>
> You work with some geospatial data for a project in your community.
> You choose the GeoTIFF format for the data.
> Your colleague asks:
>
> 1. Why did you choose the GeoTIFF format?
> 2. Does this format help to make the data FAIR?
>
>> ## Solution
>>
>> 1. You found that GeoTIFF format is the standard in your research community and
>> therefore interoperable and reusable for anyone.
>> GeoTIFF format is independent of computer’s architecture, operating system, and graphics hardware.
>> Also, the GeoTIFF format can contain both data and geographic information.
>>
>> 2. Therefore, yes, the GeoTIFF format helps to make the data FAIR.
> {: .solution}
{: .challenge}

- [HDF5](https://support.hdfgroup.org/HDF5/doc1.6/UG/03_Model.html):
The Hierarchical Data Format Version 5, (HDF5) implements a model for managing and storing data,
developed by the National Center for Supercomputing Applications (NCSA):
![HDF5]({{ page.root }}/fig/hdf5_data_model.png)

  - HDF5 is a **general-purpose**, **machine-independent** standard for storing scientific data in files.

  - HDF5 files are organized in a hierarchical structure, with two primary structures: groups and datasets.

  - HDF5 dataset: a multidimensional array of **data** elements, together with supporting **metadata**.

  - There are four essential classes of metadata: name, datatype, dataspace, and storage layout.

  - An HDF5 structure is **self-describing**, allowing an application to interpret
  the structure and contents of a file without any outside information.

> ## Why HDF5 format
>
> You work with some geospatial data for a project in your community.
> You choose the HDF5 format for the data.
> Your colleague asks:
>
> 1. Why did you choose the HDF5 format?
> 2. Does this format help to make the data FAIR?
>
>> ## Solution
>>
>> 1. You found that HDF5 format is the standard in your research community and
>> therefore interoperable and reusable for anyone.
>> HDF5 is a general-purpose, machine-independent format.
>> Also, HDF5 format can contain both data and metadata.
>>
>> 2. Therefore, yes, HDF5 format helps to make the data FAIR.
> {: .solution}
{: .challenge}

> ## Other formats for geospatial data
>
> There are many other formats to store geospatial data like
> [SHP](https://en.wikipedia.org/wiki/Shapefile)(shapefiles) for vector data,
> [DBF](https://en.wikipedia.org/wiki/.dbf)(database file), and
> [NetCDF ZARR Data](https://www.unidata.ucar.edu/blogs/developer/en/entry/netcdf-zarr-data-model-specification), etc.
{: .callout}

## Different formats for different types

There are several data types like geospatial, tabular, storyline, documentation and paper,
textual, video/audio, and image/figure.
Recommended formats for different types:

- Geospatial data: [NetCDF](https://www.unidata.ucar.edu/software/netcdf/docs/netcdf_data_model.html)
- Tabular data: [SQLite](https://www.sqlite.org/fileformat.html)
- Textual data: [Markdown](https://daringfireball.net/projects/markdown/)
- Image data: [TIFF 6.0 uncompressed](https://www.adobe.io/content/dam/udp/en/open/standards/tiff/TIFF6.pdf)
- Audio data: [Lossless Audio Codec (FLAC)](https://xiph.org/flac/)
- Video data: [MPEG-4](https://en.wikipedia.org/wiki/MPEG-4)
- Documentation: [Microsoft Word](https://en.wikipedia.org/wiki/Microsoft_Word) or [PDF](https://www.iso.org/standard/63534.html)
- Papers & Articles: [LaTeX](https://www.latex-project.org/)
- Storyline Definitions: [JSON](https://www.json.org/json-en.html)

> ## Other data types
>
> Have a look at the list of the recommended formats for different types (mentioned above)
> and pick a data type.
>
> - What are the other data formats for the type that you selected?
> - Which of those formats are common in your community?
{: .discussion}

> ## Data Management Plan
>
> Data Management Plan (DMP) covers how data can be stored, described and reused.
{: .callout}


## Different formats for different purposes

In the previous sections, we learned that different file formats have different properties.
The purpose of a file should help determine which file format to choose.
It is good to plan in the beginning of your project, what file formats to use for each purpose:

- data collection / processing / analysis,
- reuse: the longer you want to use the data, the more you have to use open, standard and
well-documented file formats to avoid obsolescence.
- preservation: many journals, archives and data repositories require that data are uploaded in certain file formats.
Therefore, you may have to keep some data files in multiple formats.

> ## Non/proprietary format
>
> File formats may be either proprietary or non-proprietary(open or free):
>
>- The proprietary format is owned by a company, or organization or individual.
>  Their specifications are usually not publicly available and the risk of obsolescence is high.
>  If you want to store data in a proprietary format for a reasonable time, consider including a readme.txt file
>  that documents the name and version of the software used to generate the file, as well as
>  the information of the company that made the software.
>
>- The open format is a file format that is published and free to be used by everybody.
{: .callout}

> ## Recommendation about data format
>
> Recently, researchers evaluated the utility of dynamical downscaling in agricultural impacts projections,
> see [their publication](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4066535/).
> They used climate data from a global climate model like CMIP3 and some
> [regional climate models](https://www.pnas.org/content/pnas/suppl/2014/05/28/1314787111.DCSupplemental/pnas.201314787SI.pdf).
> A bias correction and spatial downscaling algorithm were applied on climate data.
> Crop yield were simulated with a version of the DSSAT crop model (pDSSAT).
>
> Assume that the authors want to publish their data. What suggestions would you give the authors for data format?
>
{: .discussion}

{% include links.md %}
