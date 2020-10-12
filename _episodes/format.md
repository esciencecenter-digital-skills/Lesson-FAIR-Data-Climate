---
title: "File format"
teaching: 15
exercises: 20
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
Files are usually named as `filename.format`.
For example, climate.jpeg is a file named climate with [jpeg](https://en.wikipedia.org/wiki/JPEG) format.
You might know that `jpeg` is a commonly used format for digital images.
Therefore, the file `climate` is probably an image.

Each file type like images, video, and text can be stored in several formats.
For example, `climate.jpeg`, `climate.png`, and `climate.gif`.
All file formats are used to store image data, but they have differences in
compression, available colors, resulting filesize, etc
(for more information see [this page](https://fixthephoto.com/tech-tips/difference-between-jpeg-and-png.html)).
When deciding which one to use, it’s important to note the advantages and disadvantages of each.

Also, formats may be dependent on particular software.
When data is stored from a software program, it is usually saved in that program’s standard file format.
One example is creating tabular data using spreadsheet software.
Tabular data have specific properties that are better supported by the spreadsheet software than a word processor.

> ## no extension or multiple extensions!
>
> In [UNIX-like](https://en.wikipedia.org/wiki/UNIX-like) operating systems, a file can have no extensions,
> or more than one extension.
> For example, in `filename.tar.gz`, the `.tar` indicates that the file is a tar archive of one or more files,
> and the `.gz` indicates that the tar archive file is compressed with [gzip](https://en.wikipedia.org/wiki/Gzip).
> Also, programs reading files usually ignore the format; it is mostly intended for the human user.
> In Windows, a file should have at least one extension.
{: .callout}

> ## File formats for geospatial data in your community/research team
>
> Here are some questions about the use case you chose in the introduction.
>
> 1. What is the format of the geospatial data?
> 2. Do you know why the data is in that format?
>
{: .discussion}

## Recommended formats for different types

There are several data types like geospatial, tabular, storyline, documentation and paper,
textual, video/audio, and image/figure.
Some of them are more in line with the FAIR principles than some others.
Here are some recommended formats for different types:

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
Let's back to our example of creating tabular data using spreadsheet software.
There is no guarantee that the tabular data can be used or displayed in the future.
Because the software can become obsolete or only support a specific version of formats.

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

> ## FAIR principles
>
> Let's have a look at [FAIR principles](https://www.go-fair.org/fair-principles/).
> According to the principles, how does a file format improve FAIRness of research data?
>
>> ## Solution
>>
>> I1:(meta) data use a formal, accessible, shared, and broadly applicable language for knowledge representation.
>> For example, if data is provided in commonly understood and preferably open formats.
>>
>> R1.3: (meta)data meet domain-relevant community standards e.g. those for data formats.
> {: .solution}
{: .challenge}

## Common file formats for geospatial data

In climate-related domains e.g. weather and climate science, earth observation science, or hydrology,
data can be in many types and for different purposes.
In this section, we will explore some common data formats.

### [NetCDF](https://www.unidata.ucar.edu/software/netcdf/docs/netcdf_data_model.html):

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

> ## Choosing NetCDF format
>
> Imagine that you work with some geospatial data for a project in your community.
> You found that NetCDF format is a standard in the community.
> Your colleague asks:
>
> How does the NetCDF format improve the FAIRness of your data?
>
>> ## Solution
>>
>> The NetCDF format can contain both data and metadata.
>> It is also the standard in your community, and therefore interoperable and reusable for anyone.
> {: .solution}
{: .challenge}

### [GRIB](https://www.wmo.int/pages/prog/www/DPS/FM92-GRIB2-11-2003.pdf):

GRIB stands for general regularly-distributed information in binary.
It is **commonly used** by the [World Meteorological Organization](https://public.wmo.int/en) (WMO) for weather model data.

- The representation of the data in the GRIB format is **independent of** any particular machine representation.

- GRIB messages contain the **data** and **metadata**.

- GRIB is used operationally worldwide by most meteorological centers, for Numerical Weather Prediction output.
Some of the second-generation GRIB are used in Eumetcast of Meteosat Second Generation.
Another example is the North American Mesoscale model.

> ## Choosing GRIB format
>
> Imagine that you work with some geospatial data for a project in your community.
> You found that GRIB format is the standard in the community.
> Your colleague asks:
>
> How does the GRIB format improve the FAIRness of your data?
>
>> ## Solution
>>
>> The GRIB format is independent of any particular machine representation
>> and contains both data and metadata.
>> It is also the standard in your community, and therefore interoperable and reusable for anyone.
> {: .solution}
{: .challenge}

### [GeoTIFF](https://www.geospatialworld.net/article/geotiff-a-standard-image-file-format-for-gis-applications/):

GeoTIFF is a standard image file format to describe and store raster image data with geographic information.
So it can be used by Geographic Information System (GIS) applications.

- GeoTIFF format is suitable for a **wide range of applications worldwide**.
For example, satellite imaging systems, scanned aerial photography, scanned maps,
digital elevation models, or as a result of geographic analyses.

- It is **independent** of a computer’s architecture, operating system, and graphics hardware.

- GeoTIFF format has a three-level hierarchy: file header, image file directories, and **data**.

- GeoTIFF format stores a **broad range of georeferencing information**, catering to geographic
as well as projected coordinate systems.

- As an example, GeoTIFF 1.1 is an approved NASA Earth Science Data Systems standard
(see [Standards and Practices](https://earthdata.nasa.gov/esdis/eso/standards-and-references)).

> ## Choosing GeoTIFF format
>
> Imagine that you work with some geospatial data for a project in your community.
> You found that GeoTIFF format is the standard in the community.
> Your colleague asks:
>
> How does the GeoTIFF format improve the FAIRness of the research data?
>
>> ## Solution
>>
>> GeoTIFF format is independent of computer’s architecture, operating system, and graphics hardware.
>> and it contains both data and geographic information.
>> It is also the standard in your community, and therefore interoperable and reusable for anyone.
> {: .solution}
{: .challenge}

### [HDF5](https://www.hdfgroup.org/solutions/hdf5/):

The Hierarchical Data Format Version 5, (HDF5) implements a model for managing and storing data,
developed by the National Center for Supercomputing Applications (NCSA):
![HDF5]({{ page.root }}/fig/hdf5_data_model.png)

- HDF5 is a **general-purpose**, **machine-independent** standard for storing scientific data in files.

- HDF5 files are organized in a hierarchical structure, with two primary structures: groups and datasets.

- HDF5 dataset: a multidimensional array of **data** elements, together with supporting **metadata**.

- There are four essential classes of metadata: name, datatype, dataspace, and storage layout.

- An HDF5 structure is **self-describing**, allowing an application to interpret
the structure and contents of a file without any outside information.

- As an example, NASA's Earth Observing System, the primary data repository for
understanding global climate change, uses HDF5,
(for more information see [this page](https://www.loc.gov/preservation/digital/formats/fdd/fdd000229.shtml)).

> ## Choosing HDF5 format
>
> Imagine that you work with some geospatial data for a project in your community.
> You found that HDF5 format is the standard in the community.
> Your colleague asks:
>
> How does the HDF5 format improve the FAIRness of the research data?
>
>> ## Solution
>>
>> HDF5 is a general-purpose, machine-independent format
>> and it contains both data and metadata.
>> It is also the standard in your community, and therefore interoperable and reusable for anyone.
> {: .solution}
{: .challenge}

> ## Other formats for geospatial data
>
> There are many other formats to store geospatial data like
> [SHP](https://en.wikipedia.org/wiki/Shapefile)(shapefiles) for vector data,
> [DBF](https://en.wikipedia.org/wiki/.dbf)(database file), and
> [NetCDF ZARR Data](https://www.unidata.ucar.edu/blogs/developer/en/entry/netcdf-zarr-data-model-specification), etc.
{: .callout}

> ## Recommendation about data format
>
> Let's have a look at case-study that you selected in introduction of this tutorial,
> [here]({{ page.root }}{% link _episodes/introduction.md %}).
>
> Assume that the authors want to publish their data. What suggestions would you give the authors for data format?
>
{: .discussion}

{% include links.md %}
