# RD3_database

As part of the [Solve-RD](http://solve-rd.eu/) we are developing a metadata database to track and find samples processed by [CNAG](https://www.cnag.crg.eu/) and submitted to the [EGA](https://ega-archive.org/).

The core model for this database is designed to store sample, subject and file metadata. Using existing standards.

Datamodel:

![alt text](/datamodel/rd3_version1.jpeg "version1")

All entities are:

* Study - Container for all activities. Contains datasets
* Organisation - Organisation involved in the study
* [Subject](/datamodel/subject.md) - Human subjects, typically patients or family members
* [Sample](/datamodel/sample.md) - Samples used as input for the analysis
* File - Individual files on file systems so we can find them back, linked to the datasets describing them.
* Person 
* [Dataset](/datamodel/dataset.md) - Collection of files, collected in context of a study. Could also call this a 'fileset' if we like that better

CodeList (Ontologies)
* [anatomicalLocation](/datamodel/anatomicalLocation.md) - Code list for anatomicalLocation used for sampling. E.g. Blood
* dataUseConditions -  Code list describing different types of conditions to access the data
* disease - ICD-10 codes example_data; from C00 till C06.2
* materialType - Code list for materialType, e.g. DNA
* phenotype - Code list for phenotype, e.g. HPO term

