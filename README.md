# RD3_database

As part of the [Solve-RD](http://solve-rd.eu/) we are developing a metadata database to track and find samples processed by [CNAG](https://www.cnag.crg.eu/) and submitted to the [EGA](https://ega-archive.org/).

The core model for this database is designed to store sample, subject and file metadata. Using existing standards.

Datamodel:

![alt text](/datamodel/rd3_version1.jpeg "version1")

All entities are:

* Study - Container for all activities. Contains datasets
* Organisation - Organisation involved in the study
* [Subject]() - Human subjects, typically patients or family members
* [Sample](/datamodel/sample.md) - Samples used as input for the analysis
* File - Individual files on file systems so we can find them back, linked to the datasets describing them.
* Person 
