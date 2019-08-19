# RD3_database

As part of the [Solve-RD](http://solve-rd.eu/) we are developing a metadata database to track and find samples processed by [CNAG](https://www.cnag.crg.eu/) and submitted to the [EGA](https://ega-archive.org/).

The core model for this database is designed to store sample, subject and file metadata. Using existing standards.

##### Datamodel #####

![alt text](/datamodel/rd3_version1.jpeg "version1")

All entities are:

* [Study](/datamodel/study.md) - Container for all activities. Contains datasets
* [Organisation](/datamodel/organisation.md) - Organisation involved in the study
* [Subject](/datamodel/subject.md) - Human subjects, typically patients or family members
* [SubjectInfo](/datamodel/SubjectInfo.md) - Extra information about subject
* [Relation](/datamodel/relation.md) - Family entity relationship
* [Sample](/datamodel/sample.md) - Samples used as input for the analysis
* [File](/datamodel/file.md) - Individual files on file systems so we can find them back, linked to the datasets describing them.
* [Person](/datamodel/person.md) - Researcher or other person involved in the study  
* [Job](/datamodel/job.md) - Jobs used to process sampledata
* [Run](/datamodel/run.md) - Container of jobs
* [Dataset](/datamodel/dataset.md) - Collection of files, collected in context of a study. Could also call this a 'fileset' if we like that better
* [Disease inheritance](/datamodel/diseaseInheritance.md) - Description of known inheritance linked to disease and possibly mutation
* [Publication](/datamodel/publication.md) - Publication linked to subject and/or variant
* [LabInfo](/datamodel/LabInfo.md) - Information of process in lab (barcodes, sequencer,etc)
* [Variant](/datamodel/variant.md) - Identifier of an allele/genotype (HGVS)
* [VariantInfo](/datamodel/VariantInfo.md) - Extra information about variant
* [Library](/datamodel/Library.md) - Information for library used in experiment
 

CodeList (Ontologies)
* [anatomicalLocation](/datamodel/anatomicalLocation.md) - Code list for anatomicalLocation used for sampling. E.g. Blood
* [dataUseConditions](/datamodel/dataUseConditions.md) -  Code list describing different types of conditions to access the data
* [disease](/datamodel/disease.md) - ICD-10 codes example_data; from C00 till C06.2
* [materialType](/datamodel/materialType.md) - Code list for materialType, e.g. DNA
* [phenotype](/datamodel/phenotype.md) - Code list for phenotype, e.g. HPO term
* [Sex](/datamodel/sex.md) - code list for sex. E.g. 'M'

##### EMX #####

The default import format for [MOLGENIS](https://www.molgenis.org/) is 'EMX'. This is a flexible spreadsheet format (Excel, CSV) that allows you to annotate your data with a data model. This works because you can tell MOLGENIS the 'model' of your data via a special sheet named 'attributes'.

* [Latest version EMX](/EMX/RD3_EMX_v1.xlsx)
